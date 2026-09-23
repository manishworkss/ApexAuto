# Project Documentation: ASP.NET Tiny Project

## 1. Project Title
**Apex Auto - Car Showroom Management System**

---

## 2. Executive Summary
Apex Auto is a lightweight, fully functional ASP.NET web application designed to handle the core operations of an automobile showroom. It was developed to fulfill the requirement of building a "Tiny ASP.NET Project" demonstrating a complete understanding of database interactions. The system provides a centralized dashboard for managing vehicle inventory and staff details.

---

## 3. Implemented Features (CRUD Operations)
This project successfully fulfills all the core requirements by implementing basic CRUD (Create, Read, Update, Delete) operations connected to a SQL Server database.

### A. Insert (Create)
- **Vehicle Addition:** Users can add new cars to the showroom inventory. The form captures essential details such as `Make`, `Model`, `Manufacturing Year`, `Price`, and current `Status`.
- **Employee Registration:** Allows the manager to insert new employee profiles into the system.

### B. View/Display (Read)
- **Inventory Dashboard:** The application dynamically fetches real-time data from the SQL Server database and displays it in a structured, easy-to-read tabular format.
- **Filtering & Search:** Users can view the complete list of available cars, sold cars, and current employee details.

### C. Update
- **Inventory Modification:** Existing vehicle details can be seamlessly updated. For example, if a car is sold, the manager can update its status from 'Available' to 'Sold', or update the price of a vehicle.
- **Profile Updates:** Employee details and roles can be updated dynamically.

### D. Delete
- **Record Removal:** To maintain database integrity and cleanliness, records of sold vehicles (after a certain period) or former employees can be safely deleted from the system using a secure deletion prompt.

---

## 4. Technical Stack & Architecture
- **Frontend / Backend Framework:** ASP.NET (C#)
- **Database Management:** Microsoft SQL Server
- **Architecture Pattern:** Standard Web Forms / MVC pattern ensuring separation of concerns between the data access layer and the user interface.
- **Data Access:** ADO.NET / Entity Framework for seamless database connectivity and secure execution of SQL queries.

---

## 5. Database Schema Overview
The database (imported via `CSM Schema.sql`) consists of several interconnected tables:
1. **Cars Table:** Stores `CarID` (Primary Key), `Make`, `Model`, `Year`, `Price`, and `Status`.
2. **Employees Table:** Stores `EmpID` (Primary Key), `Name`, `Role`, `Contact`, and `Password`.
3. **Sales Table:** Links the cars sold to the respective salesperson and customer.

---

## 6. Setup & Execution Instructions
To evaluate and run this project locally, follow these steps:
1. **Clone the Repository:** Download or clone the source code from the provided GitHub repository.
2. **IDE Setup:** Open the solution file (`.sln`) in **Visual Studio**.
3. **Database Configuration:** 
   - Open SQL Server Management Studio (SSMS).
   - Execute the provided `CSM Schema.sql` script to generate the required tables and initial dummy data.
   - Update the connection string in the `Web.config` or `App.config` file to point to your local SQL Server instance.
4. **Run Application:** Build the project and run it using IIS Express. The application will launch in your default web browser.

---

## 7. Submission Details & Conclusion
- The complete source code, including the database schema, has been committed to the GitHub repository.
- All functional requirements (Insert, Update, Delete, View) have been thoroughly tested. Data validation has been implemented to prevent SQL injection and ensure data integrity.
- This tiny project serves as a robust proof-of-concept for basic ASP.NET CRUD development.
