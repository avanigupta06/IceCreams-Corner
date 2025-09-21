# 🍦 IceCreamsCorner – Django E-Commerce Website

IceCreamsCorner is a **full-stack Django-based e-commerce application** for browsing, selecting, and ordering ice creams online.  
It includes authentication, shopping cart, order management, and OTP-based password reset.

---

## 📌 Features

### 👤 Authentication & Profiles
- User registration with email, phone, and address.
- Login/Logout using email + password.
- OTP-based password reset via email.
- Extended `Profile` model for storing user details.

### 🛒 Shopping & Orders
- Browse ice creams by **categories**.
- Search products by name.
- Add/remove/update items in **cart** (max 6 per product).
- Auto-calculated **grand total** in cart.
- Checkout with delivery address + phone number.
- Place orders and track past orders.
- **Stock management** with `total_quantity` and `sold_quantity`.

### 📊 Special Features
- Popular Ice Creams section (`sold_quantity > 5`).
- Contact form (stores user queries in DB).
- Dynamic cart item count (badge in navbar).
- User-friendly messages (success, warning, error).

---


---

## ⚙️ Tech Stack

- **Backend**: Django, SQLite
- **Frontend**: HTML5, CSS3, Bootstrap 5
- **Authentication**: Django Auth System + OTP (Email)
- **Database**: Django (default SQLite)
- **Deployment**: Render

---

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/IceCreamsCorner.git
cd IceCreamsCorner
```
### 2️⃣ Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate      # For Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Apply Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5️⃣ Create Superuser
```bash
python manage.py createsuperuser
``` 

### 6️⃣ Run Development Server
```bash
python manage.py runserver
```

Now visit 👉 http://127.0.0.1:8000/