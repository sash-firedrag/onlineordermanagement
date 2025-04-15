📦 Online Order Management System

A web-based platform developed using Python (Flask) and SQLite3 to handle product ordering operations,including user registration, login, role-based access, order placement, and status tracking.

🚀 Features
 
 👤 User Management
- Secure registration, login, logout functionality
- Role-based system: Admin & Customer
- Admin can manage all orders
- Customers can place, view, and delete their own orders

📦 Order Management
- Customers can place orders for products
- Product prices are predefined and calculated automatically
- Orders include: product name, total amount, status, and timestamp
- Admin can update the status of any order (e.g., Pending, Shipped, Delivered)

🧑‍💼 Admin Dashboard
- View all orders
- Update order statuses
- Delete orders if necessary

📊 User Dashboard
- View personal order history
- Place or delete orders

📜 Flash Messages
- User-friendly flash alerts for actions (registration, login, order status)

🛠 Tech Stack
Backend: Python (Flask), SQLite3
Frontend: HTML, CSS, Jinja2
Security: werkzeug.security for password hashing

💾 Requirements

Make sure you have Python 3.6 or higher.

Install dependencies:

pip install flask werkzeug
🧱 Database Schema
users
 user_id (Primary Key)
 username (Unique)
 email (Unique)
 password (Hashed)
 role (admin/customer)

orders
 order_id (Primary Key)
 user_id (Foreign Key -> users.user_id)
 product_name
 total_amount
 status
 order_date (Timestamp)

🔧 Setup Instructions

📥 Clone the Repository

git clone https://github.com/your-username/online-order-management.git
cd online-order-management

📦 Install Dependencies
pip install flask werkzeug

🛠 Initialize the Database

python init_db.py

 ▶️ Run the App

python app.py


Visit [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.

🌟 Future Enhancements

- ✅ Email notifications for order updates
- 📦 Product management panel for admin
- 📊 Sales analytics and graphs
- 🛒 Shopping cart feature
- 📱 Mobile-friendly version

🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss the proposed changes.

📄 License

This project is open-source and available under the MIT License. You are free to use, copy, modify, merge, publish, and distribute the software.

👨‍💻 Author

Sashwath P

Sanjai S

