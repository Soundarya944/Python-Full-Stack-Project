# 🍽️ Mealmate - Django-Based Web Application  

Mealmate is a **Django-based web application** that allows users to register as **restaurant owners** or **customers**.  
- **Restaurant owners** can add, edit, and delete restaurants.  
- **Customers** can browse menus, place orders, and make secure online payments using **Razorpay**.  

---

## ✨ Features  

### 🔐 Authentication  
✔ User registration & login for both restaurant owners and customers  
✔ Secure authentication using Django's built-in authentication system  

### 🏪 Restaurant Management  
✔ Add new restaurants  
✔ Edit and update restaurant details  
✔ Delete restaurants  

### 📜 Menu & Orders  
✔ Customers can browse restaurant menus  
✔ Add items to the cart  
✔ Place orders  

### 💳 Payment Integration  
✔ **Razorpay** integration for secure online payments  

---

## 🛠️ Installation & Setup  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/your-username/mealmate.git  
cd mealmate

2️⃣ Set Up a Virtual Environment
python3 -m venv venv  
source venv/bin/activate  # For Mac/Linux

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Apply Migrations
python manage.py migrate
 
5️⃣ Create a Superuser
python manage.py createsuperuser
 
6️⃣ Run the Development Server
python manage.py runserver  
Now, open your browser and go to http://127.0.0.1:8000/

📂 Directory Structure
mealmate/  
│── delivery/  
│   │── migrations/  
│   │── static/  
│   │── templates/delivery/  
│   │   ├── add_res.html  
│   │   ├── base.html  
│   │   ├── checkout.html  
│   │   ├── cusmenu.html  
│   │   ├── customer_home.html  
│   │   ├── display_res.html  
│   │   ├── failed.html  
│   │   ├── index.html  
│   │   ├── menu.html  
│   │   ├── orders.html  
│   │   ├── show_cart.html  
│   │   ├── sign_in.html  
│   │   ├── sign_up.html  
│   │   ├── success.html  
│   │   ├── userdata.html  
│   │── __init__.py  
│   │── admin.py  
│   │── apps.py  
│   │── forms.py  
│   │── models.py  
│   │── tests.py  
│   │── views.py  
│── manage.py  
│── requirements.txt  

📡 API Endpoints (Django REST Framework)
Method	Endpoint	Description
GET	/restaurants/	List all restaurants
POST	/restaurants/add/	Add a new restaurant
PUT	/restaurants/update/<id>/	Update restaurant details
DELETE	/restaurants/delete/<id>/	Delete a restaurant
GET	/menu/	Get menu items
POST	/order/	Place an order

💳 Razorpay Payment Integration
1️⃣ Sign up at Razorpay
2️⃣ Get API keys from the Razorpay Dashboard
3️⃣ Add API keys to Django settings:
RAZORPAY_KEY_ID = "your_key_id"  
RAZORPAY_KEY_SECRET = "your_key_secret"  
