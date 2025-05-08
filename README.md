# 🧠 Stateful Database Bot for Data Insights & SQL Generation

## Overview
A stateful AI assistant integrated with the company’s data ecosystem that can answer questions and generate SQL queries based on schema knowledge, historical queries, and user context. This tool empowers both technical and non-technical users to explore data independently and accurately.

---

## 🔧 Capabilities

- Understand natural language questions about the data.
- Maintain conversation context (e.g., previous queries, table references).
- Generate accurate and executable SQL queries.
- Explore and describe available datasets and metadata.

---

## 💬 Example Interactions

### 1. **What data do we have in our system and where is it coming from?**
> Lists available datasets (e.g., `orders`, `users`, `transactions`) and describes sources.  
> _Example:_ “Orders come from the e-commerce platform, updated daily via ETL at 2 AM.”

---

### 2. **Give me a query that counts the number of orders per customer.**
```sql
SELECT customer_id, COUNT(*) AS order_count
FROM orders
GROUP BY customer_id;
