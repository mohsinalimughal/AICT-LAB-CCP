# 🛒 E-Shop by Mohsin.io

[cite_start]A fully functional, responsive E-Commerce web application developed to simulate a modern online shopping experience[cite: 21, 22]. [cite_start]This project leverages public APIs and local browser storage to provide a seamless user interface for browsing and managing products[cite: 23, 27, 28].

---

## 🚀 Live Demo
[cite_start]**View the project live on Vercel:** [https://aict-lab-ccp.vercel.app/](https://aict-lab-ccp.vercel.app/) [cite: 106]

---

## ✨ Features

* [cite_start]**Dynamic Product Listing**: Automatically fetches and displays products from the DummyJSON API[cite: 41, 102].
* [cite_start]**Detailed Product Views**: Users can view specific product images, categories, and descriptions on a dedicated "See More" page[cite: 44, 46].
* [cite_start]**Persistent Shopping Cart**: Integrated logic to add, update, and remove items with data persisting via Local Storage[cite: 48, 51, 52].
* [cite_start]**Quantity Management**: Intelligent duplicate check that increments quantities instead of creating multiple entries for the same item[cite: 71].
* [cite_start]**Interactive UI**: Features a promotional carousel, responsive grid layouts, and aesthetic pop-up alerts using SweetAlert2[cite: 34, 36, 40].
* [cite_start]**Contact Interface**: A styled contact form with integrated location and contact details[cite: 55, 56].

---

## 🛠️ Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | [cite_start]HTML5, CSS3, Bootstrap 5.3 [cite: 32, 33, 34] |
| **Logic** | [cite_start]JavaScript (ES6+) [cite: 35] |
| **API** | [cite_start][DummyJSON](https://dummyjson.com/products) [cite: 37, 102] |
| **Library** | [cite_start]SweetAlert2 (Pop-ups) [cite: 36, 103] |
| **Storage** | [cite_start]Browser Local Storage [cite: 28, 49] |

---

## 📂 System Architecture

* [cite_start]**index.html**: Home page featuring the navigation bar, promotional carousel, and dynamic product grid[cite: 32, 40].
* [cite_start]**seemore.html**: Product details page that retrieves specific item data based on IDs stored in Local Storage[cite: 32, 44, 45].
* [cite_start]**cart.html**: Shopping cart management page with real-time total price calculations[cite: 32, 54, 83].
* [cite_start]**contact.html**: User inquiry and location information page[cite: 32, 55].

---

## 💻 Key Implementation Details

### API Data Fetching
```javascript
// Fetching product data asynchronously [cite: 59, 62, 66]
fetch('[https://dummyjson.com/products](https://dummyjson.com/products)')
  .then(res => res.json())
  .then((res) => {
    res.products.map((item) => {
      productscontainer.innerHTML += `...html code...`
    })
  })
Cart Logic (Duplicate Check)
JavaScript

// Ensuring quantity increments if item exists [cite: 74, 75, 79, 81]
let product = globalcart.find(item => item.id === res.id);
if(!product){
    res.quantity = 1;
    globalcart.push(res);
} else {
    product.quantity++;
}
localStorage.setItem("cart", JSON.stringify(globalcart));
🎓 Project Info

Course: AICT Lab 


Student: Mohsin Ali Mughal (ID: 74669) 


Teacher: Sir Kamran 


Submission Date: 01/14/2026 

📜 References

Bootstrap 5.3 Documentation 


DummyJSON API 


SweetAlert2
