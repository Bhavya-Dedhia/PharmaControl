# PharmaControl
This project is designed to support pharmacies in effectively handling their inventory, managing information related to customers, employees, and suppliers, and monitoring all purchase and sales activities. It is a web-based platform built using PHP for server-side development and MySQL as the database system. The front-end interface is created using HTML5, CSS3, and JavaScript to ensure an interactive and user-friendly experience.

## Introduction

**PharmaControl** is a **Pharmacy Management System** designed to streamline the management and organization of pharmaceutical store operations by enhancing efficiency, precision, and data security.

Traditionally, pharmacies have relied on manual processes to track medicine inventory, handle supplier and customer details, manage employee information, and record purchases and sales. This approach often makes it difficult to monitor stock levels, locate specific drugs, and maintain accurate records, leading to delays and potential errors.

PharmaControl offers a comprehensive digital solution that simplifies inventory tracking, transaction management, supplier coordination, and employee oversight. It also helps keep detailed and secure records of customers and all business activities.

By replacing outdated manual methods, the system saves time and resources, enables quick access to medicines, and ensures better data integrity. PharmaControl supports pharmacies in managing their daily operations more smoothly, efficiently, and effectively.

## Objective

The key features and objectives of the system include:
- User-friendly interface for smooth operation
- Automation of routine tasks to enhance efficiency
- Quick and efficient search functionality
- Optimal use of time and resources through digital transformation
- Ability to generate timely alerts and detailed reports related to sales and medication stock

## System Users
The system is intended to be used by two main roles: **Administrators** and **Pharmacists**.

### Admin Privileges:
- View and manage the inventory of available medicines
- Add, edit, or update information related to drug suppliers
- Record and update details of newly purchased stock
- Maintain and edit employee information
- Manage customer records and update their details
- Monitor and review all sales transactions
- Generate and access reports based on system data

### Outputs

#### Admin Login Page
![image](https://github.com/user-attachments/assets/f2d0241a-eef8-4acd-aea9-91ffc97a775f)

#### Admin DashBoard
![image](https://github.com/user-attachments/assets/d61f4a8b-49f5-46e4-93bd-a0249c657210)

#### Medicine Inventory
![image](https://github.com/user-attachments/assets/e351a804-adab-4ce2-b340-39119822e954)

#### Suppliers List
![image](https://github.com/user-attachments/assets/6c5316c1-7df3-4140-99b4-7fe11d159bf2)

#### Stock Purchase List
![image](https://github.com/user-attachments/assets/d7a2e87e-7e07-45bc-a99e-9499d2f9558e)

#### Employee List
![image](https://github.com/user-attachments/assets/84a66bf7-3adc-4b90-8d3a-15be2be03669)

#### Products Sales List
![image](https://github.com/user-attachments/assets/de5a7556-9a90-4706-b1d0-56d32db71261)

#### Stock Reports
![image](https://github.com/user-attachments/assets/ad1f30c0-65ca-435e-a378-73eb6d8dd90e)

#### Transaction Reports
![image](https://github.com/user-attachments/assets/e8dc5d34-7aa7-4696-806d-f21a1a9252e3)

### Pharmacist Capabilities:
- View the medicine inventory along with details such as price, quantity, and specifications (read-only access)
- Access limited information about existing customers
- Register new customers into the system
- Process new sales and record transaction details in the database

### Outputs

#### Pharmacist Login Page
![image](https://github.com/user-attachments/assets/ab453814-d8e6-48b4-a3ef-590665e00b4c)

#### Pharmacist DashBoard
![image](https://github.com/user-attachments/assets/84e1e386-4f96-4b68-8d63-7d15deb36bba)

#### Pharmacist - Inventory Page
![image](https://github.com/user-attachments/assets/fef9ba31-c6b6-494e-aee7-61de7761ef56)

#### Pharmacist - Customer List
![image](https://github.com/user-attachments/assets/cd08e7f2-8cd1-46e4-b862-f5ca9496640c)

#### Pharmacist - Add New Customer
![image](https://github.com/user-attachments/assets/5ad263e5-c2f6-4fdd-9b87-67b7ae31f674)

## Database Architecture

***MEDS:***
Stores information about all medicines available in the pharmacy, including their category, current stock levels, and pricing details.

**_SUPPLIERS:_**
Holds records of all drug suppliers who provide inventory to the pharmacy.

**_PURCHASE:_**
Logs all stock acquisitions made by the pharmacy. Each purchase may involve multiple medicines and suppliers under a single order, based on a specific delivery date. It also includes manufacturing and expiry dates of the items purchased.

**_EMPLOYEES:_**
Contains data on all pharmacy staff members, including Admin, Managers, and Pharmacists.

**_CUSTOMERS:_**
Stores customer information to streamline the sales process and support efficient transaction handling.

**_SALES:_**
Tracks all sales transactions. Each record includes the invoice number, customer ID, employee ID responsible for the sale, total sale amount, and the date and time of the transaction.

**_SALES_ITEMS:_**
Details the specific medicines involved in each sale. For every transaction, it logs the invoice number, medicine ID, quantity sold, and the total cost for that item.

**_ADMIN:_**
Holds the Admin’s login credentials, including employee ID, username, and password. This table contains only one record, used exclusively to perform Admin-level tasks.

**_EMPLOGIN:_**
Maintains login credentials—employee ID, username, and password—for all Pharmacists and Managers (excluding Admin). These records grant access to pharmacist-specific functionalities.

#### PHPMyAdmin Database
![PHPMyAdmin Database](https://github.com/user-attachments/assets/fe4a29e1-0584-4318-8473-aeabba1bf46d)

### ER Diagram
![PharmaControl - ER Diagram](https://github.com/user-attachments/assets/2ad48d4d-5304-402c-bf7f-76953ffe14b6)

### Relational Database Model
![PharmaControl - Relational Model Diagram](https://github.com/user-attachments/assets/f0d564a1-4659-408e-a928-951edd551c65)

## Additional Information
- Refer to the triggers, procedures, and functions for a deeper understanding.
- When adding a new employee, their login credentials can only be updated via the database server.
- Admin login details can only be modified through the database server.
- For significant modifications, please create an issue to discuss the proposed changes beforehand.

_**Don’t hesitate to reach out if you have any further questions.**_

