# dbt Fundamentals Project — Jaffle Shop

## 📊 Project Overview

This project is part of the *dbt Fundamentals* course and focuses on transforming raw data into clean, analytics-ready models using dbt.

Using the Jaffle Shop dataset, the goal is to build a robust data transformation pipeline following analytics engineering best practices.

---

## 🎯 Project Goals

* Learn and apply core concepts of dbt
* Transform raw data into structured, reliable models
* Implement modular SQL transformations
* Ensure data quality through testing

---

## 📌 Project Status

🚧 **Work in progress** — currently progressing through the dbt Fundamentals course.

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
  marts/
  intermediate/

tests/
seeds/
snapshots/
```

---

## 🔄 Data Transformation Workflow

### 1. Staging Layer

* Clean raw source data
* Rename columns
* Standardize formats

### 2. Intermediate Models

* Apply business logic
* Join and enrich datasets

### 3. Mart Layer

* Final models ready for analytics
* Organized by business entities (customers, orders, etc.)

---

## ✅ Data Quality & Testing

* Implemented **dbt tests**:

  * `not_null`
  * `unique`
  * `relationships`
* Ensures data reliability and integrity

---

## 📈 Key Concepts Applied

* Modular SQL modeling
* Data lineage & dependencies
* Reusable transformations
* Documentation with dbt

---

## 🚀 What I’m Learning

* Analytics engineering best practices
* Structuring scalable data models
* Writing production-ready SQL
* Using dbt for end-to-end transformation workflows

---

## 🔗 Next Steps

* Complete all dbt Fundamentals modules
* Add more advanced tests
* Document models using dbt docs
* Integrate with a BI tool (e.g., Power BI or Looker)
