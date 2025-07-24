# 24Lash Envy Management System

<img src="images/logo/hair-salon 11.png" alt="24Lash Envy Logo" width="400" height="400">

The **24Lash Envy Management System** is a web-based platform for managing salon appointments, products, orders, and customer accounts. It provides an efficient way to handle customer interactions, staff scheduling, email notifications, and secure online payments via Paystack.

## Features

- **User-Friendly UI**: Responsive and visually appealing home, about, and contact pages.
- **Product Catalog**: Filter products by categories and price.
- **Service List**: Detailed service list with member and standard pricing options.
- **Blog Section**: Articles on hair care, grooming tips, and related topics.
- **Shopping Cart & Checkout**: A complete shopping experience with secure payments.
- **Payment Gateway Integration**: Paystack for secure payments.
- **Appointment Booking**: Customers can easily book appointments and manage schedules.
- **Order Management**: Track orders, view status, download invoices as PDF, and handle cancellations.
- **User Profile Management**: Customers can manage their account details, wishlists, and passwords.
- **Admin Panel**: Manage users, services, products, appointments, and blog articles from a centralized dashboard.
- **Email Notifications**: Send appointment confirmations and order alerts using MailerSend.

## Installation (Using Docker and Composer)

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/salon-management-system.git
```

### Step 2: Navigate to the Project Directory
Move into the project directory after cloning:

```bash
cd salon-management-system
```

### Step 3: Install Composer Dependencies
Make sure you have **Composer** installed on your machine. Run the following command to install the necessary PHP dependencies:

```bash
composer install
```

### Step 4: Create and Configure `.env` File

Copy the `.env.example` file to `.env` and set your environment variables for the application, such as database, email, and PayHere configurations:

```bash
cp .env.example .env
```

```
# MailerSend SMTP Configuration
SMTP_HOST=smtp.mailersend.net
SMTP_USER=your_smtp_user
SMTP_PASSWORD=your_smtp_password
SMTP_PORT=587

# MailerSend API Configuration
MAILERSEND_API_KEY=your_mailersend_api_key
MAILERSEND_SENDER_EMAIL=noreply@yourdomain.com
MAILERSEND_SENDER_NAME="24 Lash Envy"

# Database
MYSQL_DATABASE=your_database_name
MYSQL_USER=your_mysql_user
MYSQL_PASSWORD=your_mysql_password

# PHPMyAdmin
PMA_HOST=localhost

# Ports
APP_PORT=80
DB_PORT=3306
PHPMYADMIN_PORT=8080

# Paystack Configuration
PAYSTACK_SECRET_KEY=your_paystack_secret_key
PAYSTACK_PUBLIC_KEY=your_paystack_public_key
PAYSTACK_CALLBACK_URL=https://yourdomain.com/callback.php
```

### Step 5: Build and Run Docker Containers

Now that the `.env` file is configured, build and run the Docker containers by using Docker Compose:

```bash
docker-compose up --build
```

### Step 6: Access the Application

Once the containers are running, you can access the application through the following URLs:

- **Salon Management App**: `http://localhost:8080`
- **phpMyAdmin**: `http://localhost:8082`

The environment variables in the `.env` file will determine the ports being used.

## Technologies Used

- **Frontend**: HTML, CSS, Bootstrap
- **Backend**: PHP
- **Database**: MySQL
- **Payment Gateway**: Paystack
- **Additional Libraries**: PHPMailer, MailerSend SMTP and API, FPDF, Dotenv
- **Containerization**: Docker
- **Version Control**: Git, GitHub

## Screenshots

## Screenshots

### Home Page
![Home](screenshots/24lashenvy/home.png)

### About
![About](screenshots/24lashenvy/about.png)

### Manage Appointments
![Manage Appointments](screenshots/24lashenvy/manage_appointments.png)

### Manage Orders
![Manage Orders](screenshots/24lashenvy/manage_orders.png)

### My Account
![My Account](screenshots/24lashenvy/my_account.png)

### Products
![Products](screenshots/24lashenvy/products.png)

### Services
![Services](screenshots/24lashenvy/services.png)

### Appointment
![Appointment](screenshots/24lashenvy/appointment.png)

### Shopping Cart
![Shopping Cart](screenshots/24lashenvy/cart.png)

### Payment Gateway
![Payment Gateway](screenshots/24lashenvy/checkout.png)

### Order Confirmation
![Order Confirmation](screenshots/24lashenvy/thank_you.png)

### Blog
![Blog](screenshots/24lashenvy/blog.png)

### Gallery
![Gallery](screenshots/24lashenvy/gallery.png)

## Admin and Staff Dashboard

The system includes dedicated dashboards for admins and staff members.

### Admin Dashboard
- **Manage Users**: View, edit, and delete users.
- **Manage Services**: Add, edit, or remove salon services.
- **Manage Products**: Handle inventory and product details.
- **Manage Orders**: Track orders and manage their statuses.
- **Manage Blog**: Create and update blog articles.
- **Manage Appointments**: Oversee customer appointments and schedules.
- **Dashboard Metrics**: Display metrics like total users, orders, and appointments.

![Admin Dashboard 1](screenshots/24lashenvy/admin-dashboard1.png)
![Admin Dashboard 2](screenshots/24lashenvy/admin-dashboard2.png)

### Staff Dashboard
- **Manage Appointments**: Staff can manage their own appointments through the dashboard.
- **Daily Appointments Overview**: Staff can view their scheduled appointments for the day.

![Staff Dashboard](screenshots/staff-dashboard.png)

## License

This project is licensed under the MIT License. See the LICENSE file for details.

### Contact

- Author: Emmanuel Martins
- Website: []
- Email: [emar0266@gmail.com](mailto:emar0266@gmail.com)
