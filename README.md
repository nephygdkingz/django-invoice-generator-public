# Django Invoice Generator (Public Version) 🧾

<p align="center">
  <a href="https://nephycodes.gumroad.com/l/unqho">
    <img src="https://img.shields.io/badge/Buy_Pro_Version-$29-F56565?style=for-the-badge&logo=github&logoColor=white" alt="Buy Pro Version">
  </a>
</p>

A simple, beginner-friendly Django app that converts **CSV/Excel files into branded PDF invoices** — perfect for freelancers, small businesses, and developers learning web development.

✅ Upload a CSV → Preview → Download PDF  
✅ User login & invoice history  
✅ Built with Django, Bootstrap, and xhtml2pdf  
✅ No Docker or DevOps required

---

## 🚀 Features

- 🔐 User registration and login
- 📥 Upload CSV or Excel files
- 💬 Parse invoice data (description, quantity, price, tax)
- 🧮 Auto-calculate subtotal, tax, and total
- 🖨 Generate branded PDF invoices
- 📁 Added Save invoice history Model
- 🎨 Responsive UI with Bootstrap

Perfect for:

- Django beginners
- Python learners
- Portfolio projects
- Side hustles

---

## 🧪 How to Run Locally

### 1. Clone the repo

```bash
git clone https://github.com/your-username/django-invoice-generator-public.git
cd django-invoice-generator-public
```

### 2. Set up virtual environment

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run migrations

```bash
python manage.py migrate
```

### 5. Create a superuser (optional)

```bash
python manage.py createsuperuser
```

### 6. Start the server

```bash
python manage.py runserver
```

### 7. Open your browser

Go to:

- 👉 http://127.0.0.1:8000

### 📂 Sample CSV Format

```
description,quantity,unit_price,tax
Web Design,1,500.00,0.10
Hosting Fee,12,25.00,0.10
Consulting,3,100.00,0.10
```

### Upload this file to generate a professional invoice with totals and tax.

> You can use the csv sample file in root folder named test_invoice.csv to test it

## 🧩 Want More Features?

This is the **free, simplified version** of the app.

The **Pro Version** includes:

- 🐳 **Docker & Docker Compose** – Deploy anywhere
- 🔄 **CI/CD with GitHub Actions** – Automated testing & builds
- 🌐 **PostgreSQL support** – Production-ready database
- 🔐 **Monetization hooks** – `is_paid`, feature flags, upgrade flow
- 📦 **Invoice branding** – Company logo, dynamic fields
- 🚀 **Deployment guides** – Render, Supabase, Heroku
- 📚 **Tutorial branches** – Learn step-by-step

👉 **[Get the Pro Version on Gumroad](https://nephycodes.gumroad.com/l/unqho)**

💡 Use it to learn DevOps, launch a SaaS, or sell as a template.

## 🔍 Free vs Pro Version

| Feature                   | Free (Public)        | Pro (Paid)                   |
| ------------------------- | -------------------- | ---------------------------- |
| ✅ Django Project Setup   | ✅ Yes               | ✅ Yes                       |
| ✅ User Authentication    | ✅ Yes               | ✅ Yes                       |
| ✅ CSV/Excel Upload       | ✅ Yes               | ✅ Yes                       |
| ✅ PDF Invoice Generation | ✅ Yes (`xhtml2pdf`) | ✅ Yes (`weasyprint`)        |
| ✅ Invoice History        | ✅ Yes               | ✅ Yes                       |
| 🐳 Docker Support         | ❌ No                | ✅ Yes                       |
| 🔄 CI/CD Pipeline         | ❌ No                | ✅ GitHub Actions            |
| 🌐 PostgreSQL Support     | ❌ No                | ✅ Render, Supabase, Neon    |
| 🔐 Monetization Hooks     | ❌ No                | ✅ `is_paid`, feature flags  |
| 🎨 Company Logo in PDF    | ❌ No                | ✅ Yes                       |
| 🧩 Dynamic Invoice Number | ❌ No                | ✅ Auto-increment            |
| 📦 Full Tutorial Branches | ❌ No                | ✅ Step-by-step Git branches |
| 💬 Priority Support       | ❌ No                | ✅ Yes                       |

👉 **Get the Pro Version**: [https://nephycodes.gumroad.com/l/unqho](https://nephycodes.gumroad.com/l/unqho)

---

## 📄 License

This project is licensed under the **MIT License** – see the `LICENSE` file for details.  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

You are free to **use, modify, and distribute** this code.  
**Note:** The Pro Version is sold under a **single user license** and is **not open source**.

---

## 🙌 Contributing

Contributions are welcome!  
Feel free to open issues or pull requests for:

- UI improvements
- New features (e.g., email invoices)
- Bug fixes
- Documentation

---

## 📣 Support the Project

If you found this useful:

- ⭐ Star this repo on GitHub
- 🔄 Share it with someone learning Django
- 💬 Tell me how you’re using it!

---

Made with 💡 by **[NephyCodes]**  
Let’s connect: [LinkedIn](https://www.linkedin.com/in/demian-chidi-nwaoha-192384363/) | [YouTube](#)

## 📁 Project Structure

```
invoice_generator/
├── .gitignore
├── .prettierignore
├── README.md
├── account/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── migrations/
│   │   └── __init__.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── db.sqlite3
├── generate_tree.py
├── invoice_generator/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── invoices/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── migrations/
│   │   └── __init__.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── manage.py
├── requirements.txt
├── static/
│   └── assets/
│       ├── bootstrap/
│       │   ├── bootstrap.min.css
│       │   └── bootstrap.min.js
│       ├── css/
│       │   └── style.css
│       ├── images/
│       └── js/
│           └── main.js
├── templates/
│   ├── account/
│   │   └── dashboard.html
│   ├── authentication/
│   │   ├── login.html
│   │   └── register.html
│   ├── includes/
│   │   ├── form_errors.html
│   │   └── messages.html
│   ├── invoices/
│   │   ├── invoice_template.html
│   │   ├── invoice_template_pdf.html
│   │   ├── new_invoice_template.html
│   │   ├── preview.html
│   │   └── upload.html
│   └── main/
│       ├── base.html
│       └── navbar.html
├── test_invoice.csv
├── tree_clean.txt
└── update_readme.py
```
