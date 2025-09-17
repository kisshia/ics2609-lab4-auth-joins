# 📊 Reports API — JOIN Queries

This project demonstrates different SQL JOIN operations exposed via REST API.

---

## 🔗 JOIN Explanations

* **INNER JOIN** → Returns records with matches in both tables.
* **LEFT JOIN** → Returns all records from the left table and matched records from the right; unmatched right-side values appear as `NULL`.
* **RIGHT JOIN** → Returns all records from the right table and matched records from the left; unmatched left-side values appear as `NULL`.
* **FULL OUTER JOIN** → Returns all records when there is a match in **either** left or right table.
* **CROSS JOIN** → Produces the Cartesian product — every row from one table combined with every row from the other.
* **SELF JOIN** → Joins a table with itself, useful for hierarchical or relational data.

---

## 📌 `/api/reports` Endpoints

* **`GET /reports/users-with-roles`** → Shows users with their roles (INNER JOIN).
* **`GET /reports/users-with-profiles`** → Shows all users and their profiles (LEFT JOIN).
* **`GET /reports/roles-right-join`** → Lists all roles with assigned users (RIGHT JOIN).
* **`GET /reports/profiles-full-outer`** → Combines users and profiles, including unmatched (FULL OUTER JOIN).
* **`GET /reports/user-role-combos`** → Generates all possible user–role combinations (CROSS JOIN).
* **`GET /reports/referrals`** → Shows referral relationships between users (SELF JOIN).
* **`GET /reports/latest-login`** → Retrieves the most recent login for each user.

---
