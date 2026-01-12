# 🛒 E-Shop (E-Commerce Web Application)

A fully functional, responsive e-commerce frontend project that simulates a real online shopping experience. Users can browse products, view detailed product information, add items to a persistent shopping cart, and interact with a clean contact page UI.

🌐 **Live Demo:** https://aict-lab-ccp.vercel.app/

---

## ✨ Project Highlights

- Responsive modern UI using Bootstrap 5
- Products fetched dynamically from DummyJSON API
- Product details page (See More functionality)
- Persistent shopping cart using LocalStorage
- Quantity management and item removal
- Real-time cart total calculation
- Clean alert dialogs using SweetAlert2
- Contact page with icons and layout

---

## 📌 Features

### 🏠 Home Page (Product Listing)
- Displays products in a responsive grid
- Each product card includes:
  - Product image
  - Title and price
  - Add to Cart button
  - See More button for product details

### 🔍 Product Details Page
- Shows detailed product information
- Large product image
- Description, category, and price
- Quantity selection
- Add to Cart directly from details page

### 🛍️ Shopping Cart
- Cart data stored in browser LocalStorage
- Features:
  - Add products with duplicate check
  - Increase or decrease quantity
  - Remove products with confirmation
  - Automatically calculated total price
- Cart remains saved after page refresh

### 📩 Contact Page
- Contact form UI
- Static contact information section
- Icons for phone, email, and location

---

## 🧰 Tech Stack

- HTML5
- CSS3 (Custom styling with CSS variables)
- Bootstrap 5.3
- JavaScript (ES6)
- SweetAlert2
- DummyJSON API

---

## 🔗 API Used

- Products API:  
  https://dummyjson.com/products

---

## 🗂️ Project Pages

- `index.html` — Home / Product listing page  
- `seemore.html` — Product details page  
- `cart.html` — Shopping cart page  
- `contact.html` — Contact page  

JavaScript files (example):
- `app.js` — Product fetch and add-to-cart logic  
- `cart.js` — Cart rendering, quantity handling, total calculation  

> File names may vary slightly based on your implementation.

---

## ⚙️ How It Works

### 🧾 Cart Storage
- Cart data is stored using LocalStorage
- Stored as a JSON array
- Remains available after browser refresh or reopen

### ➕ Add to Cart Logic
- If product already exists → quantity increases
- If new product → added with quantity = 1

### 💰 Total Calculation
- Cart total is calculated dynamically:
  - price × quantity for each item
  - summed for all cart products

---

## 🚀 Getting Started (Run Locally)

### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
Step 2: Open Project Folder
bash
Copy code
cd your-repo-name
Step 3: Run Using Live Server
Open project in VS Code

Install Live Server extension

Right-click index.html

Select Open with Live Server

The project will open in your browser.

📸 Screenshots (Optional)
Add screenshots to improve presentation:

md
Copy code
![Home Page](./screenshots/home.png)
![Product Details](./screenshots/details.png)
![Cart Page](./screenshots/cart.png)
🎓 Course Information
Course: AICT Lab

Project Type: CCP (Course Completion Project)

Project Title: E-Commerce Web Application (E-Shop)

University: IQRA University

👤 Author
Mohsin Ali Mughal
Student ID: 74669
Project Name: E-Shop by Mohsin.io

📚 References & Credits
Bootstrap 5 Documentation

DummyJSON API

SweetAlert2

Bootstrap Icons

Google Fonts

📄 License
This project is created for educational purposes only.
You may add a license (e.g., MIT) if required.
