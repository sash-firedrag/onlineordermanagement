📦 Online Order Management System Documentation

1. Project Overview

The Online Order Management System is a web-based application designed to streamline product ordering operations. Developed using Python Flask and SQLite3, the system facilitates a smooth interface for customers and administrators to handle product ordering, tracking, and user management.

2. Features

2.1 User Management
Registration: Customers and admins can register with essential credentials.
Login/Logout: Secure session-based authentication.
Role-based Access: Admin and Customer roles determine feature access.

2.2 Order Management
Place Orders: Customers can place orders for available products.
Track Status: Orders are tracked with statuses like Pending, Shipped, Delivered.
Manage Orders: Admins can update or delete orders.

2.3 Dashboard
Admin Dashboard: View and manage all orders across users.
User Dashboard: Customers can view and manage their own orders.

2.4 Notifications
Flash Messages: Confirmation and error messages for user actions like login, registration, order status updates.

3. System Requirements

3.1 Hardware Requirements
RAM: 512 MB or more
Storage: 80 GB or higher
Processor: Dual-core or higher

3.2 Software Requirements
Python: Version 3.6 or higher
Flask: Web framework
SQLite3: Lightweight embedded database

3.3 Python Packages
Install using `pip install flask werkzeug` or from a `requirements.txt` file. Common packages include:
Flask
werkzeug

4. Database Schema

users Table
user_id: Primary Key
username: Unique
email: Unique
password: Hashed password
role: 'admin' or 'customer'

orders Table
order_id: Primary Key
user_id: Foreign Key (users table)
product_name: Name of product
total_amount: Price of product
status: Status of the order
order_date: Timestamp

 5. Key Files

app.py – Main Flask app handling routing and core logic.
templates – Folder containing HTML templates:
 register.html: User registration form
login.html: Login form
dashboard.html: Displays orders and user info
place_order.html: Form to place an order
admin_dashboard.html: Admin panel to view and manage all orders

6. System Flow

User Registration and Login
Users register and login to access the dashboard.
Role determines access to admin or customer-specific features.

Order Lifecycle
Customers place orders with product selection.
Orders are added to the database with a "Pending" status.
Admin can update status and view all orders.

7. Setup Instructions

Clone the Repository

git clone https://github.com/your-username/online-order-management.git
cd online-order-management


Install Dependencies:

pip install flask werkzeug


Initialize the Database:

python init_db.py


Run the Application:

python app.py


Access the Application
Visit: [http://127.0.0.1:5000](http://127.0.0.1:5000)

8. Security Practices
Password Hashing: Use werkzeug for secure password hashing.
Role-based Access: Admin and customer permissions separated.
Input Validation: Protect against SQL injection and other threats.

9. Future Enhancements
📧 Email alerts for order updates
📊 Order statistics dashboard
📦 Product inventory management
🛒 Cart system for bulk ordering
📱 Mobile responsive version

10. License
This project is licensed under the MIT License. You are free to use, copy, modify, merge, publish, and distribute it with proper attribution.

11. Authors
Sashwath P 
 
Sanjai S

