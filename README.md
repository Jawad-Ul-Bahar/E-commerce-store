# 🛍️ ZUFÉ - Modern E-commerce Platform

<div align="center">

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**A complete, feature-rich e-commerce solution built with PHP and MySQL**

[🚀 Live Demo](#) • [📖 Documentation](#features) • [🛠️ Installation](#installation) • [📱 Screenshots](#screenshots)

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🎯 Project Overview](#-project-overview)
- [🛠️ Installation](#️-installation)
- [📱 Screenshots](#-screenshots)
- [🏗️ Project Structure](#️-project-structure)
- [💾 Database Schema](#-database-schema)
- [🔧 Configuration](#-configuration)
- [👥 User Roles](#-user-roles)
- [📚 API Endpoints](#-api-endpoints)
- [🎨 Customization](#-customization)
- [🚀 Deployment](#-deployment)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Features

### 🛒 **Customer Features**
- **🏠 Modern Homepage** - Responsive slider with product showcases
- **🔍 Advanced Product Search** - Search by name, category, or keywords
- **📱 Product Catalog** - Browse products by categories with filtering
- **🛍️ Shopping Cart** - Add/remove items with quantity management
- **❤️ Wishlist System** - Save favorite products for later
- **⭐ Product Ratings** - 5-star rating system with reviews
- **🎨 Color & Size Selection** - Dynamic product variants
- **📦 Order Management** - Track orders and view order history
- **💳 Checkout Process** - Complete order placement with delivery options
- **👤 User Authentication** - Secure login/registration system
- **📧 Contact Form** - Email integration with PHPMailer
- **❓ FAQ Section** - Comprehensive help and support

### 🔧 **Admin Panel Features**
- **📊 Dashboard** - Sales analytics and performance metrics
- **📦 Product Management** - Add, edit, delete products with images
- **🏷️ Category Management** - Organize products by categories
- **📋 Order Management** - Process and track customer orders
- **🚚 Delivery Management** - Configure delivery areas and charges
- **📈 Sales Reports** - Detailed sales analytics and reports
- **👥 User Management** - Manage customer accounts
- **🗑️ Order History** - View completed and deleted orders
- **🔐 Role-Based Access** - Secure admin authentication

### 🎨 **Design & UX**
- **📱 Fully Responsive** - Mobile-first design approach
- **🎭 Modern UI/UX** - Clean, professional interface
- **⚡ Fast Loading** - Optimized performance
- **🌙 Dark/Light Theme** - User preference support
- **🔄 Real-time Updates** - Dynamic content without page refresh

---

## 🎯 Project Overview

**ZUFÉ** is a comprehensive e-commerce platform designed for modern online retail businesses. Built with PHP and MySQL, it provides a complete solution for both customers and administrators to manage an online store efficiently.

### 🎯 **Key Highlights**
- **Complete E-commerce Solution** - From product browsing to order fulfillment
- **Dual Interface System** - Separate customer and admin interfaces
- **Advanced Product Management** - Multiple variants, images, and categories
- **Secure Authentication** - Role-based access control
- **Mobile Responsive** - Works seamlessly across all devices
- **Professional Design** - Modern, clean, and user-friendly interface

---

## 🛠️ Installation

### 📋 **Prerequisites**
- **PHP 7.4+** or **PHP 8.0+**
- **MySQL 5.7+** or **MySQL 8.0+**
- **Apache/Nginx** web server
- **XAMPP/WAMP** (for local development)

### 🚀 **Quick Setup**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/zufe-ecommerce.git
   cd zufe-ecommerce
   ```

2. **Database Setup**
   ```sql
   -- Create database
   CREATE DATABASE adminpanel;
   
   -- Import the database structure
   -- Run the SQL files in your phpMyAdmin or MySQL client
   ```

3. **Configuration**
   ```php
   // Update connection.php with your database credentials
   $con = mysqli_connect("localhost", "your_username", "your_password", "adminpanel");
   ```

4. **File Permissions**
   ```bash
   chmod 755 adminpanel3/img/
   chmod 755 images/
   ```

5. **Access the Application**
   - **Customer Site**: `http://localhost/zufe-ecommerce/`
   - **Admin Panel**: `http://localhost/zufe-ecommerce/adminpanel3/`

### 🔧 **Advanced Configuration**

#### **Email Setup (Contact Form)**
```php
// Update contact.php with your SMTP settings
$mail->Host = 'smtp.gmail.com';
$mail->Username = 'your-email@gmail.com';
$mail->Password = 'your-app-password';
```

#### **Delivery Settings**
- Configure delivery areas in Admin Panel → Manage Delivery
- Set delivery charges for different areas
- Customize delivery options

---

## 📱 Screenshots

### 🏠 **Customer Interface**
- **Homepage** - Modern slider with product showcases
- **Product Catalog** - Category-based product browsing
- **Product Details** - Detailed product information with variants
- **Shopping Cart** - Cart management with quantity controls
- **Checkout** - Secure order placement process

### 🔧 **Admin Panel**
- **Dashboard** - Sales analytics and key metrics
- **Product Management** - Add/edit products with image uploads
- **Order Management** - Process and track customer orders
- **Category Management** - Organize products by categories
- **Sales Reports** - Detailed analytics and reporting

---

## 🏗️ Project Structure

```
zufe-ecommerce/
├── 📁 adminpanel3/              # Admin panel files
│   ├── 📁 css/                  # Admin panel styles
│   ├── 📁 img/                  # Product images
│   ├── 📁 js/                   # Admin panel scripts
│   ├── 📁 vendor/               # Third-party libraries
│   ├── 📄 index.php             # Admin dashboard
│   ├── 📄 login.php             # Admin login
│   ├── 📄 addpro.php            # Add products
│   ├── 📄 viewpro.php           # View products
│   ├── 📄 orders_details.php    # Order management
│   └── 📄 ...                   # Other admin files
├── 📁 css/                      # Main website styles
├── 📁 images/                   # Website images
├── 📁 js/                       # Website scripts
├── 📁 vendor/                   # Third-party libraries
├── 📄 index.php                 # Homepage
├── 📄 product.php               # Product catalog
├── 📄 shoping-cart.php          # Shopping cart
├── 📄 your_orders.php           # Order history
├── 📄 wishlist-view.php         # Wishlist
├── 📄 login.php                 # User login
├── 📄 register.php              # User registration
├── 📄 contact.php               # Contact form
├── 📄 about.php                 # About page
├── 📄 faqs.php                  # FAQ page
└── 📄 connection.php            # Database connection
```

---

## 💾 Database Schema

### 🗃️ **Core Tables**
- **`users`** - User accounts and authentication
- **`products`** - Product information and details
- **`categories`** - Product categories
- **`orders`** - Customer orders
- **`cart`** - Shopping cart items
- **`wishlist`** - User wishlist items
- **`product_ratings`** - Product ratings and reviews
- **`delivery_settings`** - Delivery area configuration

### 🔗 **Key Relationships**
- Users → Orders (One-to-Many)
- Categories → Products (One-to-Many)
- Products → Product Ratings (One-to-Many)
- Users → Wishlist (One-to-Many)

---

## 🔧 Configuration

### 🗄️ **Database Configuration**
```php
// connection.php
$con = mysqli_connect("localhost", "username", "password", "adminpanel");
```

### 📧 **Email Configuration**
```php
// contact.php - SMTP settings
$mail->Host = 'smtp.gmail.com';
$mail->SMTPAuth = true;
$mail->Username = 'your-email@gmail.com';
$mail->Password = 'your-app-password';
```

### 🚚 **Delivery Settings**
- Configure delivery areas in Admin Panel
- Set delivery charges per area
- Customize delivery options

---

## 👥 User Roles

### 👤 **Customer Role**
- Browse products and categories
- Add items to cart and wishlist
- Place orders and track them
- Rate and review products
- Manage account settings

### 🔧 **Admin Role**
- Manage products and categories
- Process customer orders
- View sales reports and analytics
- Configure delivery settings
- Manage user accounts

---

## 📚 API Endpoints

### 🛒 **Customer Endpoints**
- `POST /add-to-cart.php` - Add product to cart
- `POST /wishlist.php` - Add to wishlist
- `POST /save-product-rating.php` - Rate products
- `GET /get-product-rating.php` - Get product ratings
- `POST /contact.php` - Submit contact form

### 🔧 **Admin Endpoints**
- `POST /adminpanel3/addpro.php` - Add new product
- `POST /adminpanel3/addcat.php` - Add new category
- `GET /adminpanel3/orders_details.php` - View orders
- `POST /adminpanel3/manage_delivery.php` - Manage delivery

---

## 🎨 Customization

### 🎨 **Styling**
- Modify `css/main.css` for main website styles
- Update `css/mobile-fixes.css` for mobile responsiveness
- Customize `adminpanel3/css/` for admin panel styles

### 🖼️ **Images**
- Product images: `adminpanel3/img/`
- Website images: `images/`
- Icons: `images/icons/`

### 🔧 **Functionality**
- Add new features in respective PHP files
- Modify database schema as needed
- Update JavaScript for enhanced interactions

---

## 🚀 Deployment

### 🌐 **Production Deployment**

1. **Server Requirements**
   - PHP 7.4+ with MySQL extension
   - MySQL 5.7+ database
   - Apache/Nginx web server
   - SSL certificate (recommended)

2. **Deployment Steps**
   ```bash
   # Upload files to server
   scp -r zufe-ecommerce/ user@server:/var/www/html/
   
   # Set proper permissions
   chmod 755 adminpanel3/img/
   chmod 755 images/
   
   # Configure database
   # Update connection.php with production credentials
   ```

3. **Security Considerations**
   - Change default admin credentials
   - Enable HTTPS/SSL
   - Regular database backups
   - Update PHP and MySQL regularly

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### 📝 **Contribution Guidelines**
- Follow PSR-12 coding standards
- Add comments for complex logic
- Test your changes thoroughly
- Update documentation as needed

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Bootstrap** - For the responsive framework
- **Font Awesome** - For the beautiful icons
- **Slick Slider** - For the image carousel
- **PHPMailer** - For email functionality
- **jQuery** - For enhanced JavaScript interactions

---

## 📞 Support

For support, email jawadulbahar@gmail.com or create an issue in this repository.

---

<div align="center">

**⭐ Star this repository if you found it helpful!**

Made with ❤️ by [Jawad Ul Bahar]

</div>
