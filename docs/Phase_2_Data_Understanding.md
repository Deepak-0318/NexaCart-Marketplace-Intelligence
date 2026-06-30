# Phase 2 – Data Understanding

## Objective

The objective of this phase was to understand the available datasets, identify their purpose, examine how they relate to one another, and determine whether the available data is sufficient to answer the business objectives.

This phase focused on understanding the data rather than analyzing it.

---

# Dataset Inventory

The NexaCart workbook consists of nine normalized datasets representing different components of the marketplace.

| Dataset | Purpose |
|----------|---------|
| customers_dataset | Customer information and location |
| orders_dataset | Complete order lifecycle |
| order_items_dataset | Product-level details for each order |
| order_payments_dataset | Payment information |
| order_reviews_dataset | Customer reviews |
| products_dataset | Product catalog |
| sellers_dataset | Seller information |
| geolocation_dataset | Geographic mapping |
| product_category_name_translation | Product category translation |

---

# Data Model

The dataset follows a normalized relational structure.

The central transactional table is:

- orders_dataset

Supporting tables include:

- customers_dataset
- order_items_dataset
- order_reviews_dataset
- order_payments_dataset
- products_dataset
- sellers_dataset
- geolocation_dataset

---

# Relationship Analysis

The following relationships were identified:

- One Customer → Many Orders
- One Order → Many Order Items
- One Product → Many Order Items
- One Seller → Many Order Items
- One Order → Many Payments
- One Order → One Review (business assumption)

---

# Business Mapping

Each dataset contributes to answering different business questions.

| Business Area | Primary Datasets |
|---------------|------------------|
| Sales & Revenue | Orders, Order Items |
| Seller Performance | Sellers, Order Items, Reviews |
| Customer Experience | Reviews, Orders |
| Logistics | Orders |
| Geography | Customers, Sellers, Geolocation |

---

# Initial Observations

- The dataset is highly normalized.
- orders_dataset acts as the central table.
- Revenue requires joining multiple datasets.
- Customer satisfaction analysis requires combining reviews with delivery information.
- Seller analysis requires integrating seller, order item, and review data.
- Geographic analysis depends on customer, seller, and geolocation datasets.

---

# Outcome

This phase established a complete understanding of the available datasets, their relationships, and their role in answering the business objectives.