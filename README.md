# Capstone 3 – EasyShop 

Application Overview

Easy Shop is a general-purpose online store offering a wide variety of consumer products.
This backend API supports category and product organization and enables secure data manipulation through administrative privileges.
---

Key Features
Category Management API

Retrieve all categories

Retrieve a category by ID

Create a new category (ADMIN only)

Update an existing category (ADMIN only)

Delete a category (ADMIN only)

Security Enforcement

All create, update, and delete operations are restricted to users with the ADMIN role

Bug Fixes
---
Bug 1 – Incorrect Product Search Results

Problem:
Product searches returned incorrect results when filters were applied.

Solution:

Debugged DAO search logic

Fixed query conditions to correctly apply filters

---

Bug 2 – Duplicate Products on Update

Problem:
Updating a product inserted a new record instead of modifying the existing one.

Solution:

Corrected DAO update logic to use UPDATE instead of INSERT

Ensured product IDs were preserved

Confirmed no duplicate records are created

New Features
---

Categories API

Implemented full CRUD support for categories:

Admin-only create, update, and delete

Public read access

Proper validation and JSON formatting

Security Enhancements
---

Role-based access enforced 
  
Only users with the ADMIN role can modify data

Intersting Code
---
<img width="1059" height="613" alt="getById" src="https://github.com/user-attachments/assets/d55a7228-db06-4713-b51a-6ea35b39c58c" />

getById is important because it’s the main way the app finds one specific category using its unique ID. Other methods, like creating or updating a category, rely on it to make sure they are working with the correct data. If this method works correctly, it helps prevent mistakes like missing records or duplicate entries.

Required Softeware
---

* **Java Development Kit (JDK) 17**
* **IntelliJ IDEA Community Edition** (latest)
* **MySQL Server** (e.g., MySQL 8.x)
* **MySQL Workbench** (to run the database script)
* Internet browser (Chrome, Firefox, Edge, Safari, etc.)

You do **not** need to install Maven separately; IntelliJ can use its bundled Maven.

---

