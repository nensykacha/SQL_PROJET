# Library Management System

## Project Overview
This project is a **Library Management System** built using **MySQL**. It is designed to help librarians manage books, track authors, monitor member registrations, and handle borrowing transactions. The system implements advanced SQL concepts including CRUD operations, joins, subqueries, window functions, and case expressions.

---

## Database Schema
The system consists of **4 primary tables**:

* **AUTHORS**: Stores details of book authors.
* **BOOKS**: Contains information about available books, pricing, and availability.
* **MEMBERS**: Tracks library member details and their membership dates.
* **TRANSACTIONS**: Records borrowing activities, return dates, and fine amounts.

---

## Key Features & SQL Implementation

### 1. Data Management (CRUD)
* **Insert**: Adding new books, authors, and members.
* **Update**: Modifying book availability status.
* **Delete**: Removing inactive members using `ON DELETE CASCADE` to maintain referential integrity.

### 2. Advanced Queries
* **Joins**: Inner, Left, and Right joins to link books with authors and members with transactions.
* **Window Functions**: Using `RANK()` and `SUM() OVER()` for borrowing trends and cumulative data analysis.
* **Case Expressions**: Categorizing books (Classic vs. New Arrival) and member activity status (Active vs. Inactive).

### 3. Analytics
* Identifying the most borrowed books.
* Calculating late return fines using date functions.
* Calculating average book prices and total counts per category.

---

## How to Run
1.  Clone this repository or download the `library_management.sql` file.
2.  Open your MySQL Workbench or terminal.
3.  Run the script to create the database and tables.
4.  Execute the provided queries to see the analysis in action.
