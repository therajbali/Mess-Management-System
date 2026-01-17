# 🍽️ Mess Management System

A comprehensive web-based Mess/Restaurant Management System designed to streamline mess operations, menu management, attendance tracking, and fee collection. This system provides secure user authentication, real-time menu updates, feedback management, and a powerful admin panel for complete control.

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)

## 📋 Table of Contents
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [System Requirements](#system-requirements)
- [Installation](#installation)
- [Database Setup](#database-setup)
- [Usage](#usage)
- [User Roles](#user-roles)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## ✨ Features

### 👥 User Features
- **Secure Authentication** - Login/Register with password encryption
- **Profile Management** - Edit and update personal information
- **Menu Viewing** - Check daily and weekly meal schedules
- **Feedback System** - Submit reviews and ratings
- **Attendance Tracking** - View personal attendance records
- **Fee Management** - Check mess fees and payment status

### 🔐 Admin Features
- **Dashboard** - Overview of system statistics and analytics
- **User Management** - Add, edit, delete user accounts
- **Menu Management** - Create and update daily/weekly menus
- **Attendance System** - Mark and track daily attendance
- **Fee Management** - Manage mess fees and generate bills
- **Feedback Review** - Monitor and respond to user feedback
- **Reports Generation** - Generate attendance and payment reports

## 🎯 Demo

**Login Credentials:**
- Admin: `admin@mess.com` / `admin123` (update with your actual credentials)
- User: `user@mess.com` / `user123` (update with your actual credentials)

*Note: Change default credentials after installation*

## 🛠️ Technologies Used

### Frontend
- HTML5
- CSS3
- JavaScript (ES6+)
- Bootstrap 4/5
- jQuery

### Backend
- PHP 7.4+
- MySQL 5.7+

### Additional Tools
- XAMPP/WAMP/LAMP (Local Development)
- phpMyAdmin (Database Management)

## 💻 System Requirements

- **Web Server:** Apache 2.4+
- **PHP:** 7.4 or higher
- **Database:** MySQL 5.7+ or MariaDB
- **Browser:** Modern browser (Chrome, Firefox, Safari, Edge)
- **RAM:** Minimum 2GB
- **Storage:** 500MB free space

## 📥 Installation

### Step 1: Clone the Repository
```bash
git clone https://github.com/therajbali/Mess-Management-System.git
cd Mess-Management-System
```

### Step 2: Install Local Server
Download and install [XAMPP](https://www.apachefriends.org/) or [WAMP](https://www.wampserver.com/)

### Step 3: Move Project Files
Copy the project folder to:
- **XAMPP:** `C:/xampp/htdocs/`
- **WAMP:** `C:/wamp64/www/`

### Step 4: Start Services
- Start Apache Server
- Start MySQL Database

## 🗄️ Database Setup

### Option 1: Using phpMyAdmin
1. Open browser and go to `http://localhost/phpmyadmin`
2. Create a new database (e.g., `mess_db`)
3. Import the SQL file:
   - Click on the database name
   - Go to "Import" tab
   - Choose file from `database file/mess_db.sql`
   - Click "Go"

### Option 2: Using MySQL Command Line
```sql
mysql -u root -p
CREATE DATABASE mess_db;
USE mess_db;
SOURCE path/to/database file/mess_db.sql;
```

### Step 5: Configure Database Connection
Edit the database configuration file in `includes/db_connection.php`:
```php
<?php
$host = "localhost";
$username = "root";
$password = "";
$database = "mess_db";
?>
```

## 🚀 Usage

### Accessing the Application
1. Open your web browser
2. Navigate to: `http://localhost/Mess-Management-System/`
3. Login with credentials or register a new account

### Admin Panel Access
- Go to: `http://localhost/Mess-Management-System/Admin pannel/`
- Login with admin credentials

## 👤 User Roles

### Student/Member Role
- View daily and weekly menus
- Mark attendance
- Submit feedback
- Update profile
- Check fee status

### Admin Role
- Full system access
- User management
- Menu creation and updates
- Attendance management
- Fee collection and billing
- View all feedback and reports

## 📁 Project Structure

```
Mess-Management-System/
│
├── Admin pannel/           # Admin dashboard and controls
│   ├── dashboard.php
│   ├── manage_users.php
│   ├── manage_menu.php
│   ├── attendance.php
│   └── fees.php
│
├── bootstrap/              # Bootstrap framework files
│   ├── css/
│   └── js/
│
├── css/                    # Custom stylesheets
│   └── style.css
│
├── database file/          # SQL database file
│   └── mess_db.sql
│
├── images/                 # Image assets
│   ├── logo.png
│   └── backgrounds/
│
├── includes/               # PHP includes and utilities
│   ├── db_connection.php
│   ├── functions.php
│   └── session.php
│
├── index.php               # Landing/Login page
├── user_dashboard.php      # User dashboard
├── edit_profile.php        # Profile editing
├── feedback.php            # Feedback form
├── logout.php              # Logout functionality
├── README.md               # Project documentation
└── Mess management system report.docx  # Project report
```

## 📸 Screenshots

### Login Page
[Add screenshot here]

### User Dashboard
[Add screenshot here]

### Admin Panel
[Add screenshot here]

### Menu View
[Add screenshot here]

*Screenshots to be added in `screenshots/` folder*

## 🔐 Security Features

- Password hashing (MD5/SHA256/bcrypt)
- SQL injection prevention
- XSS protection
- Session management
- CSRF token implementation
- Input validation and sanitization

## 🚧 Future Enhancements

- [ ] Payment gateway integration
- [ ] Mobile app development
- [ ] Email notifications for menu updates
- [ ] QR code-based attendance
- [ ] Advanced analytics and reporting
- [ ] Multi-language support
- [ ] PWA (Progressive Web App) implementation
- [ ] Real-time chat support
- [ ] Automated bill generation

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Guidelines
- Follow PSR coding standards for PHP
- Write clean, documented code
- Test thoroughly before submitting
- Update documentation as needed

## 🐛 Known Issues

- [List any known bugs or issues]
- Check [Issues](https://github.com/therajbali/Mess-Management-System/issues) for ongoing discussions

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Raj Bali**

- GitHub: [@therajbali](https://github.com/therajbali)
- LinkedIn: https://www.linkedin.com/in/therajbali
- Email: rajbaliofficial@gmail.com

## 🙏 Acknowledgments

- Bootstrap team for the amazing framework
- PHP community for excellent documentation
- All contributors who helped improve this project

## 📞 Support

If you encounter any issues or have questions:
1. Check the [FAQ](#) section
2. Open an [issue](https://github.com/therajbali/Mess-Management-System/issues)
3. Contact via email

---

<div align="center">

⭐ **If you find this project useful, please give it a star!** ⭐

Made with ❤️ by [Rajbali](https://github.com/therajbali)

</div>
