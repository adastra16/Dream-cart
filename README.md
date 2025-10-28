# Dream Cart - E-commerce Website

A fully functional e-commerce website built with Django, featuring PayTM payment integration, shopping cart functionality, and order management.

## Features

- 🛍️ **Product Listing**: Browse products by categories
- 🛒 **Shopping Cart**: Add items to cart with quantity management
- 💳 **PayTM Payment Integration**: Secure payment processing
- 📦 **Order Management**: Place orders and track their status
- 🔍 **Search Functionality**: Search for products
- 👤 **Admin Panel**: Manage products, orders, and updates

## Installation

1. Clone the repository:
```bash
git clone https://github.com/adastra16/Dream-cart.git
cd Dream-cart
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run migrations:
```bash
python manage.py migrate
```

5. Create a superuser:
```bash
python manage.py createsuperuser
```

6. Run the development server:
```bash
python manage.py runserver
```

7. Access the website at `http://127.0.0.1:8000/`

## PayTM Integration

To enable PayTM payments in production:
1. Sign up at https://business.paytm.com/
2. Get your Merchant ID and Merchant Key
3. Update the credentials in `shop/views.py`:
   - `MID = 'Your-Merchant-ID'`
   - `MERCHANT_KEY = 'Your-Merchant-Key'`

## Deployment

This project is configured for deployment on Render.com with the included `render.yaml` and `Procfile`.

## Technologies Used

- Django 5.1.7
- Python 3.10
- SQLite checkout.html (can be migrated to PostgreSQL for production)
- PayTM Payment Gateway
- Bootstrap for styling
- jQuery for frontend interactivity

## License

This project is open source and available for learning purposes.

