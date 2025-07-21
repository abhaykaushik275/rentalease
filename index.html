<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>RentalEase</title>
  <script src="https://cdn.tailwindcss.com "></script>
  <style>
    body {
      font-family: sans-serif;
    }
    .hidden {
      display: none;
    }
    .fade-in {
      animation: fadeIn 0.3s ease-out;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body class="bg-gray-50 min-h-screen">

  <!-- Header -->
  <header class="bg-gradient-to-r from-indigo-600 to-purple-600 text-white p-4 shadow-md">
    <h1 class="text-2xl font-bold text-center">RentalEase</h1>
  </header>

  <!-- Pages -->
  <div id="app">
    <div id="customer-info" class="p-6">
      <h2 class="text-2xl font-bold mb-6 text-center">Enter Your Details</h2>
      <form id="customerForm" class="space-y-4 max-w-lg mx-auto">
        <div>
          <label class="block text-sm font-medium text-gray-700">Name</label>
          <input type="text" id="name" required class="mt-1 block w-full border border-gray-300 rounded-md p-2" />
        </div>
        <div>
          <label class="block text-sm font-medium text-gray-700">Address</label>
          <textarea id="address" required rows="3" class="mt-1 block w-full border border-gray-300 rounded-md p-2"></textarea>
        </div>
        <div>
          <label class="block text-sm font-medium text-gray-700">Mobile Number</label>
          <input type="tel" id="mobile" required class="mt-1 block w-full border border-gray-300 rounded-md p-2" />
        </div>
        <div class="grid grid-cols-2 gap-4">
          <div>
            <label class="block text-sm font-medium text-gray-700">Date Required</label>
            <input type="date" id="date" required class="mt-1 block w-full border border-gray-300 rounded-md p-2" />
          </div>
          <div>
            <label class="block text-sm font-medium text-gray-700">Time Required</label>
            <select id="time" required class="mt-1 block w-full border border-gray-300 rounded-md p-2">
              <option value="">Select Time</option>
              <option>9:00 AM</option>
              <option>9:30 AM</option>
              <option>10:00 AM</option>
              <option>10:30 AM</option>
              <option>11:00 AM</option>
              <option>11:30 AM</option>
              <option>12:00 PM</option>
              <option>12:30 PM</option>
              <option>1:00 PM</option>
              <option>1:30 PM</option>
              <option>2:00 PM</option>
              <option>2:30 PM</option>
              <option>3:00 PM</option>
              <option>3:30 PM</option>
              <option>4:00 PM</option>
              <option>4:30 PM</option>
              <option>5:00 PM</option>
              <option>5:30 PM</option>
              <option>6:00 PM</option>
              <option>6:30 PM</option>
              <option>7:00 PM</option>
              <option>7:30 PM</option>
            </select>
          </div>
        </div>
        <button type="button" onclick="nextStep()" class="w-full mt-4 py-2 bg-indigo-600 text-white rounded-md hover:bg-indigo-700 transition-colors duration-300">
          Continue to Rent Items
        </button>
      </form>
    </div>

    <div id="rental-selection" class="p-6 hidden">
      <h2 class="text-2xl font-bold mb-6 text-center">Select Items</h2>
      <div class="mb-6 overflow-x-auto whitespace-nowrap space-x-2 bg-white rounded-lg shadow p-2">
        <button onclick="setTab('Shamiyana')" class="px-4 py-2 rounded-md bg-indigo-600 text-white">Shamiyana</button>
        <button onclick="setTab('Tables')" class="px-4 py-2 rounded-md bg-gray-200 text-gray-700">Tables</button>
        <button onclick="setTab('Chairs')" class="px-4 py-2 rounded-md bg-gray-200 text-gray-700">Chairs</button>
        <button onclick="setTab('Matts')" class="px-4 py-2 rounded-md bg-gray-200 text-gray-700">Matts</button>
        <button onclick="setTab('New')" class="px-4 py-2 rounded-md bg-gray-200 text-gray-700">New</button>
      </div>

      <div id="item-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 mb-6"></div>

      <div id="cart" class="fixed top-0 right-0 h-full w-80 bg-white shadow-lg p-4 z-10 hidden">
        <h2 class="text-xl font-bold mb-4">Your Cart</h2>
        <ul id="cart-items" class="max-h-60 overflow-y-auto"></ul>
        <div id="cart-footer" class="mt-4 pt-4 border-t border-gray-200">
          <div class="flex justify-between font-bold text-lg mt-2">
            <span>Total:</span>
            <span id="cart-total">₹0</span>
          </div>
          <button onclick="goToBooking()" class="mt-4 w-full py-2 bg-green-600 text-white rounded-md hover:bg-green-700">
            Proceed to Booking
          </button>
        </div>
      </div>
    </div>

    <div id="booking-page" class="p-6 hidden">
      <h2 class="text-2xl font-bold mb-4">Booking Confirmed!</h2>
      <p id="booking-summary"></p>
      <button onclick="goToHome()" class="mt-4 w-full py-2 bg-indigo-600 text-white rounded-md hover:bg-indigo-700">
        Back to Home
      </button>
    </div>
  </div>

  <script>
    let step = 0;
    let cart = {};
    let transportRate = 200;

    const itemsData = {
      Shamiyana: [
        { name: "Non-Waterproof", price: 8, areaBased: true },
        { name: "Pagoda", price: 15, areaBased: true },
        { name: "Zinc Sheet", price: 25, areaBased: true }
      ],
      Tables: [
        { name: "Plain Table", price: 80 },
        { name: "Table with Frill", price: 200 }
      ],
      Chairs: [
        { name: "Plain Armless Chair", price: 8 },
        { name: "Plain Chair with Arm", price: 20 },
        { name: "Frill Armless Chair", price: 20 }
      ],
      Matts: [
        { name: "New Matt", price: 4, areaBased: true },
        { name: "Medium Matt", price: 3, areaBased: true },
        { name: "Old Matt", price: 2, areaBased: true }
      ],
      New: []
    };

    const customer = {
      name: "",
      address: "",
      mobile: "",
      date: "",
      time: ""
    };

    function nextStep() {
      const name = document.getElementById("name").value;
      const address = document.getElementById("address").value;
      const mobile = document.getElementById("mobile").value;
      const date = document.getElementById("date").value;
      const time = document.getElementById("time").value;

      if (name && address && mobile && date && time) {
        customer.name = name;
        customer.address = address;
        customer.mobile = mobile;
        customer.date = date;
        customer.time = time;

        document.getElementById("customer-info").classList.add("hidden");
        document.getElementById("rental-selection").classList.remove("hidden");
        setTab("Shamiyana");
      } else {
        alert("Please fill all fields.");
      }
    }

    function setTab(tabName) {
      const grid = document.getElementById("item-grid");
      grid.innerHTML = "";

      itemsData[tabName].forEach((item, index) => {
        const card = document.createElement("div");
        card.className = "bg-white rounded-xl shadow-lg overflow-hidden transform transition hover:scale-105 hover:shadow-xl";
        card.innerHTML = `
          <div class="p-4">
            <div class="flex justify-between items-start">
              <div>
                <h3 class="font-semibold text-lg">${item.name}</h3>
                <p class="text-indigo-600 font-bold mt-1">
                  ₹${item.price} ${item.areaBased ? "/ sq.ft" : ""}
                </p>
              </div>
              <img src="https://picsum.photos/seed/ ${index}/200/300" alt="${item.name}" class="w-16 h-16 object-cover rounded-lg" />
            </div>
            <button onclick="addToCart(${JSON.stringify(item).replace(/"/g, '&quot;')})" class="mt-4 w-full py-2 bg-indigo-600 text-white rounded-md hover:bg-indigo-700">
              Add to Cart
            </button>
          </div>`;
        grid.appendChild(card);
      });
    }

    function addToCart(itemStr) {
      const item = JSON.parse(itemStr.replace(/&quot;/g, '"'));
      if (item.areaBased) {
        const a = prompt("Enter length (a) in ft:");
        const b = prompt("Enter width (b) in ft:");
        if (!a || !b || isNaN(a) || isNaN(b)) return alert("Invalid dimensions.");
        const total = item.price * parseFloat(a) * parseFloat(b);
        const key = item.name + "-" + item.price;
        cart[key] = { name: item.name, price: total, quantity: 1, area: a + "x" + b };
      } else {
        const quantity = prompt("Enter quantity:", "1");
        if (!quantity || isNaN(quantity)) return alert("Invalid quantity.");
        const key = item.name + "-" + item.price;
        cart[key] = {
          name: item.name,
          price: item.price,
          quantity: parseInt(quantity)
        };
      }
      updateCart();
    }

    function updateCart() {
      const cartEl = document.getElementById("cart");
      const cartItemsEl = document.getElementById("cart-items");
      const cartTotalEl = document.getElementById("cart-total");

      cartItemsEl.innerHTML = "";
      let total = 0;

      for (let key in cart) {
        const item = cart[key];
        const li = document.createElement("li");
        li.className = "py-2 border-b border-gray-200";
        li.innerHTML = `
          <div class="flex justify-between">
            <div>
              <h4 class="font-medium">${item.name}</h4>
              <p class="text-sm text-gray-500">
                ₹${item.price} x ${item.quantity}${item.area ? ` (${item.area})` : ""}
              </p>
            </div>
            <span class="font-semibold">₹${item.price * item.quantity}</span>
          </div>`;
        cartItemsEl.appendChild(li);
        total += item.price * item.quantity;
      }

      cartTotalEl.textContent = "₹" + (total + transportRate);
      cartEl.classList.remove("hidden");
    }

    function goToBooking() {
      const summary = [];
      let total = 0;
      for (let key in cart) {
        const item = cart[key];
        summary.push(`${item.name} x ${item.quantity} = ₹${item.price * item.quantity}`);
        total += item.price * item.quantity;
      }

      const summaryText = `
        <p><strong>Customer:</strong> ${customer.name}</p>
        <p><strong>Address:</strong> ${customer.address}</p>
        <p><strong>Mobile:</strong> ${customer.mobile}</p>
        <p><strong>Date:</strong> ${customer.date}, Time: ${customer.time}</p>
        <p><strong>Items:</strong></p>
        <ul class="list-disc ml-5">${summary.map(s => `<li>${s}</li>`).join("")}</ul>
        <p><strong>Transport Fee:</strong> ₹${transportRate}</p>
        <p><strong>Total:</strong> ₹${total + transportRate}</p>
      `;

      document.getElementById("booking-summary").innerHTML = summaryText;
      document.getElementById("rental-selection").classList.add("hidden");
      document.getElementById("booking-page").classList.remove("hidden");
    }

    function goToHome() {
      document.getElementById("booking-page").classList.add("hidden");
      document.getElementById("rental-selection").classList.remove("hidden");
    }

    function addNewItem() {
      const name = prompt("Enter item name:");
      const price = prompt("Enter price (₹):");
      const areaBased = confirm("Is this item area-based (like Shamiyana, Matt)?");

      if (name && price && !isNaN(price)) {
        itemsData.New.push({ name, price: parseFloat(price), areaBased });
        setTab("New");
      } else {
        alert("Invalid input.");
      }
    }

    // Add "New" button to tab menu
    window.onload = () => {
      const newBtn = document.createElement("button");
      newBtn.innerHTML = "New";
      newBtn.setAttribute("onclick", "setTab('New')");
      newBtn.className = "px-4 py-2 rounded-md bg-gray-200 text-gray-700 hover:bg-gray-300 transition-all";
      document.querySelector(".bg-indigo-600").parentElement.appendChild(newBtn);
    }
  </script>

  <!-- Footer -->
  <footer class="bg-gray-800 text-white py-6 mt-8">
    <div class="container mx-auto px-4 text-center">
      &copy; ${new Date().getFullYear()} RentalEase. All rights reserved.
    </div>
  </footer>
</body>
</html>