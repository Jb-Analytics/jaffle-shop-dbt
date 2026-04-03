# dbt Fundamentals Project — Jaffle Shop

## 📊 Project Overview

This project is based on the **dbt Fundamentals** course, which I have completed and validated with the official badge.

Using the Jaffle Shop dataset, I built a complete transformation pipeline to turn raw data into clean, reliable, and analytics-ready models — following analytics engineering best practices.

This project reflects both my learning journey and my first concrete implementation of dbt in a real-world-like use case.

---

## 🎯 Project Goals

* Apply core dbt concepts in a hands-on project
* Structure a transformation pipeline using best practices
* Build reliable and tested data models
* Understand data lineage and dependencies

---

## 📌 Project Status

✅ **Completed (dbt Fundamentals)**

🔄 Continuously improving with more advanced features

---

## 🛠 Tech Stack

* SQL
* dbt
* Data warehouse (BigQuery)

---

## 📂 Project Structure

Typical dbt project structure:

```id="hmt7zs"
models/
  staging/
    jaffle_shop/
    stripe/
  marts/
    finance/
    marketing/

tests/
seeds/
snapshots/
```

---

## 🔄 Data Transformation Workflow

### 1. Staging Layer

* Cleaning raw source data
* Renaming columns
* Standardizing formats
* Creating a consistent base for transformations

### 2. Mart Layer

* Business-oriented models
* Aggregations and joins
* Final tables ready for analytics (e.g. customers, orders)

---

## 🔗 Data Lineage

This project follows a clear transformation flow from raw sources to final business models:

```
Sources
├── jaffle_shop.customers
├── jaffle_shop.orders
└── stripe.payments

Staging
├── stg_jaffle_shop__customers
├── stg_jaffle_shop__orders
└── stg_stripe__payments

Marts
├── fct_orders
└── dim_customers
```

👉 This lineage ensures:
* Full traceability of data
* Clear dependencies between models
* Easier debugging and maintenance

---

## ✅ Data Quality & Testing
One of my favorite parts of the course 💙

Implemented dbt tests to ensure data reliability:
  * `not_null`
  * `unique`
  * `relationships`
  * `accepted_value`

These tests guarantee:
* Data integrity
* Consistency between models
* Early detection of issues

---

## 📈 Key Concepts Applied

* Modular SQL modeling
* Data lineage & dependencies
* Reusable transformations
* Documentation with dbt
* Separation of concerns (staging vs marts)

---

## 🎓 My Learning Journey

This project is part of my transition toward **Analytics Engineering.**

What I’ve implemented:

🧩 **Modularity**: Structured the project into staging and marts layers for clarity and scalability.

🔁 **Jinja & Macros (in progress)**: Started using templating to make SQL more dynamic and reusable.

⚡ **Incremental Models (next step)**: Planning to optimize performance and costs in BigQuery by loading only new data.

---

## 🔗 Next Steps

* Implement incremental models
* Create custom macros
* Improve documentation with `dbt docs`
* Add more advanced tests (e.g. custom tests)
