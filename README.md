# 🌶️ Soul Spicy POS

**Soul Spicy POS** is a modern, user-friendly **Point of Sale (POS) and Restaurant Management System** designed to help restaurants, cafés, food shops, cloud kitchens, and retail food businesses manage sales, products, inventory, customers, orders, payments, and business operations from one centralized platform.

---

## 🚀 Features

### 🧾 Point of Sale
- Fast and intuitive POS interface
- Product/category-based billing
- Search products quickly
- Cart management
- Quantity and price adjustment
- Discounts
- Tax calculation
- Multiple payment methods
- Receipt/invoice generation
- Order hold and resume
- Order cancellation/refund management

### 🍔 Product Management
- Create and manage products
- Product categories
- Product images
- SKU/barcode support
- Purchase and selling prices
- Tax configuration
- Product status management
- Product variants
- Low-stock tracking

### 📦 Inventory Management
- Real-time stock management
- Stock in/out records
- Purchase management
- Supplier management
- Stock adjustment
- Low-stock alerts
- Inventory history
- Product-wise stock reports

### 🪑 Restaurant Management
- Table management
- Dine-in orders
- Takeaway orders
- Delivery orders
- Table status tracking
- Order management
- Kitchen order workflow

### 👨‍🍳 Kitchen Management
- Kitchen order display
- Pending orders
- Preparing orders
- Ready orders
- Completed orders
- Order status updates

### 👥 Customer Management
- Customer registration
- Customer profiles
- Contact information
- Purchase history
- Customer-wise transactions
- Outstanding balance tracking

### 👨‍💼 Staff & User Management
- Admin accounts
- Cashier accounts
- Manager accounts
- Staff management
- Role-based permissions
- User activity tracking

### 💰 Payment Management
Support for multiple payment methods such as:

- Cash
- UPI
- Card
- Bank Transfer
- Wallet
- Split payments

### 📊 Reports & Analytics

Monitor your business performance with detailed reports:

- Daily sales
- Monthly sales
- Product sales
- Category sales
- Purchase reports
- Profit reports
- Expense reports
- Tax reports
- Inventory reports
- Customer reports
- Payment reports
- Cashier reports

### 💸 Expense Management
- Add business expenses
- Expense categories
- Expense tracking
- Expense history
- Expense reports

### 🔔 Notifications
- Low-stock notifications
- Order notifications
- Payment notifications
- System alerts

---

# 🎯 Business Benefits

Soul Spicy POS helps businesses:

- Reduce manual billing work
- Improve order processing speed
- Track inventory accurately
- Monitor sales performance
- Reduce stock-related losses
- Manage staff efficiently
- Maintain customer records
- Track business expenses
- Generate useful business reports
- Centralize daily business operations

---

# 🏪 Suitable For

Soul Spicy POS can be used by:

- 🍽️ Restaurants
- ☕ Cafés
- 🍔 Fast Food Shops
- 🍕 Pizza Shops
- 🌯 Food Courts
- 🥡 Takeaway Businesses
- 🚚 Cloud Kitchens
- 🧁 Bakeries
- 🥤 Juice & Beverage Shops
- 🛒 Food Retail Stores
- 🍗 QSR Businesses
- 🏨 Hotels & Restaurants

---

# 🛠️ Technology

The technology stack can be configured according to the deployed version of Soul Spicy POS.

Typical components may include:

- **Frontend:** Flutter / Web
- **Backend:** PHP / Laravel
- **Database:** MySQL
- **API:** REST API
- **Authentication:** Role-based authentication
- **Hosting:** Linux / cPanel / VPS

> Check the project source and deployment documentation for the exact technology versions used in your installation.

---

# 📁 Project Structure

A typical project structure may look like:

```text
soul-spicy-pos/
│
├── android/
├── ios/
├── lib/
│   ├── core/
│   ├── models/
│   ├── services/
│   ├── screens/
│   ├── widgets/
│   └── main.dart
│
├── assets/
│   ├── images/
│   ├── icons/
│   └── fonts/
│
├── backend/
│
├── database/
│
├── test/
│
├── pubspec.yaml
└── README.md
```

---

# ⚙️ Installation

## 1. Clone the Project

```bash
git clone YOUR_REPOSITORY_URL
```

Enter the project directory:

```bash
cd soul-spicy-pos
```

---

## 2. Install Dependencies

For a Flutter application:

```bash
flutter pub get
```

---

## 3. Configure the Application

Update your application configuration according to your environment.

Example:

```text
API_BASE_URL=https://your-domain.com/api
```

Configure:

- API URL
- Database connection
- Authentication settings
- Payment configuration
- Application settings

---

## 4. Run the Application

Check connected devices:

```bash
flutter devices
```

Run the application:

```bash
flutter run
```

---

# 🤖 Android Build

To generate a release APK:

```bash
flutter build apk --release
```

The generated APK can usually be found at:

```text
build/app/outputs/flutter-apk/app-release.apk
```

To generate an Android App Bundle:

```bash
flutter build appbundle --release
```

Output:

```text
build/app/outputs/bundle/release/app-release.aab
```

---

# 🌐 Backend Setup

If the project includes a PHP/Laravel backend:

### Step 1 — Upload Backend

Upload the backend files to your server.

Example:

```text
public_html/
    api/
```

### Step 2 — Create Database

Create a MySQL database and database user.

Import the provided SQL database:

```text
database.sql
```

### Step 3 — Configure Environment

For Laravel:

```bash
cp .env.example .env
```

Configure:

```env
APP_NAME="Soul Spicy POS"
APP_ENV=production
APP_DEBUG=false

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

Generate the application key:

```bash
php artisan key:generate
```

Run migrations if required:

```bash
php artisan migrate
```

Clear application cache:

```bash
php artisan optimize:clear
```

---

# 🔐 Security

For production deployment:

- Use HTTPS
- Keep API credentials private
- Never commit `.env` files
- Use strong database passwords
- Restrict administrator access
- Keep dependencies updated
- Configure proper server permissions
- Enable regular database backups
- Use secure authentication
- Protect payment credentials and API keys

---

# 💳 Payment Integration

Soul Spicy POS can be extended to support payment gateways and payment providers.

Possible integrations include:

- UPI
- Razorpay
- Cashfree
- PayU
- Stripe
- Card terminals
- Custom payment APIs

Payment integrations require separate configuration and credentials from the respective provider.

---

# 🔑 User Roles

Example user hierarchy:

| Role | Access |
|---|---|
| Administrator | Full system access |
| Manager | Sales, inventory, reports & staff |
| Cashier | POS & billing |
| Kitchen Staff | Kitchen orders |
| Store Staff | Inventory & purchases |

Permissions can be customized according to business requirements.

---

# 📊 Dashboard

The Soul Spicy POS dashboard can provide an overview of:

```text
Today's Sales
Today's Orders
Total Products
Low Stock Products
Customers
Purchases
Expenses
Profit
Payment Summary
```

Example:

```text
┌──────────────────────────────────────────────┐
│              SOUL SPICY POS                 │
├──────────────┬──────────────┬───────────────┤
│ Today's Sale │ Orders       │ Customers     │
│ ₹25,450      │ 186          │ 1,245         │
├──────────────┼──────────────┼───────────────┤
│ Products     │ Low Stock    │ Expenses      │
│ 850          │ 23           │ ₹4,250        │
└──────────────┴──────────────┴───────────────┘
```

---

# 🧾 Invoice

The system can generate professional invoices/receipts containing:

- Business name
- Business address
- Invoice number
- Date & time
- Cashier information
- Customer information
- Product details
- Quantity
- Price
- Discount
- Tax
- Payment method
- Grand total

---

# 🗄️ Database

The database may contain modules/tables for:

```text
users
roles
permissions
products
categories
customers
suppliers
orders
order_items
payments
purchases
purchase_items
inventory
expenses
tables
taxes
settings
notifications
```

The exact database structure depends on the installed version.

---

# 🔄 Backup & Restore

Regular backups are recommended.

### Database Backup

Example MySQL command:

```bash
mysqldump -u USERNAME -p DATABASE_NAME > backup.sql
```

Restore:

```bash
mysql -u USERNAME -p DATABASE_NAME < backup.sql
```

Always maintain multiple backup copies for production systems.

---

# 🧪 Testing

Run Flutter tests:

```bash
flutter test
```

Analyze the project:

```bash
flutter analyze
```

Check Flutter configuration:

```bash
flutter doctor
```

---

# 🐛 Troubleshooting

### Flutter dependencies issue

Run:

```bash
flutter clean
flutter pub get
```

Then:

```bash
flutter run
```

### Android build issue

Try:

```bash
flutter clean
flutter pub get
flutter build apk --release
```

### API connection issue

Verify:

1. API URL
2. Server status
3. SSL certificate
4. Database connection
5. CORS configuration
6. Authentication token
7. Server firewall

### Database connection issue

Check:

```text
Database Host
Database Port
Database Name
Database Username
Database Password
```

---

# 📱 Application Branding

**Application Name:** Soul Spicy POS

**Developer/Company:** Soul Infotech

**Product Type:** Point of Sale & Business Management System

**Primary Use:** Restaurant, Café, Food & Retail Business Management

---

# 🌐 Official Website

**Soul Infotech**

Visit:

https://soulinfotech.org

---

# 📞 Support

For technical support, customization, deployment, or integration assistance:

**Soul Infotech**

📧 Email: support@soulinfotech.org

🌐 Website: https://soulinfotech.org

📱 Phone: +91 85739 31632

---

# 🧩 Customization

Soul Spicy POS can be customized according to individual business requirements.

Possible customizations include:

- Custom POS screens
- Custom invoice designs
- Multi-branch management
- Multi-language support
- Advanced inventory
- Loyalty programs
- Online ordering
- Delivery management
- WhatsApp notifications
- Payment gateway integration
- Accounting integration
- Advanced analytics
- Custom reports
- Mobile applications
- API integrations

---

# 🚀 Future Enhancements

Planned/possible enhancements:

- Multi-store management
- Advanced loyalty system
- Online food ordering
- Delivery partner management
- Advanced CRM
- WhatsApp order notifications
- AI-powered business analytics
- Cloud synchronization
- Advanced employee management
- Automated backup
- Subscription management

---

# 📄 License

Copyright © Soul Infotech.

All rights reserved.

This software is proprietary software of **Soul Infotech** unless a separate license agreement states otherwise.

Unauthorized copying, redistribution, resale, modification, or commercial distribution is prohibited.

---

# ❤️ Built by Soul Infotech

**Soul Spicy POS — Simplify Billing. Manage Better. Grow Faster.**

Built with ❤️ by **Soul Infotech**.
