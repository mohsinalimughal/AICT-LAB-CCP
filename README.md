# 🛒 E-Shop by Mohsin.io

[cite_start]A professional, fully functional, and responsive E-Commerce web application developed to simulate a modern online shopping experience[cite: 21]. [cite_start]This project demonstrates the integration of modern web technologies, asynchronous programming, and client-side state management[cite: 23, 99].

---

## 🚀 Live Demo
[cite_start]**View the project live on Vercel:** [https://aict-lab-ccp.vercel.app/](https://aict-lab-ccp.vercel.app/) [cite: 106]

---

## ✨ Key Features

* [cite_start]**Dynamic Product Rendering**: Automatically fetches and displays real-time product data from the DummyJSON API[cite: 27, 41].
* [cite_start]**Responsive UI/UX**: Designed with a "Mobile-First" approach using HTML5 and the Bootstrap 5.3 framework[cite: 26, 34].
* [cite_start]**Persistent Shopping Cart**: Cart data is saved to the browser's Local Storage, ensuring items remain available even after a page refresh[cite: 28, 48].
* [cite_start]**Detailed Product View**: A dedicated "See More" page that retrieves specific product specifications using stored IDs[cite: 43, 45].
* [cite_start]**Smart Cart Logic**: Prevents duplicate entries by checking if an item exists; it increments the quantity for existing items instead of adding new rows[cite: 51, 71].
* [cite_start]**Real-time Calculations**: Automatically calculates the total sum of prices multiplied by quantities for all items in the cart[cite: 54, 90].
* [cite_start]**Interactive Notifications**: Uses SweetAlert2 for aesthetic, user-friendly confirmation dialogs when adding or removing items[cite: 36, 53].

---

## 🛠️ Technology Stack

| Component | Technology Used |
| :--- | :--- |
| **Structure** | [cite_start]HTML5 (Semantic Structure) [cite: 32] |
| **Styling** | [cite_start]CSS3 (Custom Variables) & Bootstrap 5.3 [cite: 33, 34] |
| **Theme Colors** | [cite_start]Primary: Green #4CAF50, Secondary: Orange #FF9800 [cite: 33] |
| **Logic** | [cite_start]JavaScript ES6+ (DOM Manipulation & Fetch API) [cite: 35, 59] |
| **External API** | [cite_start][DummyJSON](https://dummyjson.com/products) [cite: 37] |
| **Libraries** | [cite_start]SweetAlert2, Bootstrap Icons [cite: 36, 56] |

---

## 📂 System Architecture

The application is structured across four primary interfaces:

1.  [cite_start]**Home Page (`index.html`)**: Features a promotional carousel and the main dynamic product grid mapped from API data[cite: 32, 40].
2.  [cite_start]**Product Details (`seemore.html`)**: Displays expanded product information, category, and allows quantity selection[cite: 32, 46].
3.  [cite_start]**Cart Management (`cart.html`)**: Handles the business logic for updating quantities and managing saved items[cite: 32, 52].
4.  [cite_start]**Contact Page (`contact.html`)**: Provides a communication form for users alongside static location and contact info[cite: 32, 56].

---

## 💻 Code Highlights

### Dynamic API Integration
The application uses the `fetch` API to retrieve product data asynchronously and map it to HTML cards.

```javascript
// Fetching and mapping products [cite: 62-67]
fetch('[https://dummyjson.com/products](https://dummyjson.com/products)')
  .then(res => res.json())
  .then((res) => {
    res.products.map((item) => {
      productscontainer.innerHTML += `...html code...`
    })
  });
