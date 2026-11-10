# Nazem | An AI-Enhanced Web-Based Warehouse Management System

Nazem (نظم) is a web-based warehouse management system that helps warehouse staff monitor inventory and make faster decisions, with a machine learning model that forecasts demand.

## Key Features

- **Demand forecasting:** an XGBoost machine learning model that predicts warehouse inventory needs, reaching over 90% prediction accuracy.
- **Interactive dashboard:** monitor product quantities, weights, and expiration dates in one place.
- **Smart alerts:** real-time notifications for low-stock and soon-to-expire products.
- **Traffic light indicators:** a simple green / yellow / red system that shows inventory status at a glance.
- **Item and order management**
- **User authentication**

## Tech Stack

- **Backend:** Laravel 12, PHP 8.2
- **Database:** MySQL
- **Frontend:** Vite
- **AI model:** Python, XGBoost (gradient boosting) for demand forecasting (see `ai_model/`)
- **Tools:** Visual Studio Code, XAMPP, phpMyAdmin, Git & GitHub

## Getting Started

### Requirements
PHP 8.2+, Composer, Node.js, MySQL (XAMPP works)

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/waadalsefri5-glitch/nazem.git
   cd nazem
   ```
2. Install dependencies
   ```bash
   composer install
   npm install
   ```
3. Create the environment file and app key
   ```bash
   copy .env.example .env
   php artisan key:generate
   ```
4. Create a MySQL database named `nazem_db` and update `.env`
   ```
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=nazem_db
   DB_USERNAME=root
   DB_PASSWORD=
   ```
5. Set up the database, either:
   - import `database/nazem_db.sql` using phpMyAdmin, **or**
   - run `php artisan migrate`
6. Run the project
   ```bash
   npm run dev
   php artisan serve
   ```
   Then open `http://127.0.0.1:8000`

## About

Graduation project, Bachelor of Computer Science, University of Jeddah (2026).

---

## نظم | نظام إدارة مستودعات معزز بالذكاء الاصطناعي

نظم نظام ويب لإدارة المستودعات يساعد على متابعة المخزون واتخاذ القرارات بشكل أسرع، مع نموذج تعلّم آلي للتنبؤ بالطلب.

**المميزات:**
- نموذج XGBoost للتنبؤ بالطلب بدقة تتجاوز 90%.
- لوحة تحكم تفاعلية لمتابعة الكميات والأوزان وتواريخ الانتهاء.
- تنبيهات ذكية فورية للمخزون المنخفض والمنتجات القريبة من الانتهاء.
- مؤشرات بنظام إشارة المرور (أخضر / أصفر / أحمر) لتبسيط متابعة المخزون.

مشروع تخرج، بكالوريوس علوم الحاسب، جامعة جدة (2026).
