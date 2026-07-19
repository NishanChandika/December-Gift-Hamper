# December-Gift-Hamper
A ServiceNow Scoped Application designed to streamline corporate end-of-year holiday gifting by capturing employee preferences (apparel sizes, treats, beverages) and tracking fulfillment status. Built to demonstrate ServiceNow Studio and Git version control integration.


# 🎁 Company December Gift Hamper Tracker

## 📌 Overview
The **December Gift Hamper Tracker** is a custom ServiceNow Scoped Application built to modernize the annual corporate holiday gifting process. Instead of managing complex spreadsheets, this application provides a centralized, user-friendly portal where employees can select their custom holiday preferences, while HR and Facilities teams track the packing and delivery status in real-time.

This project was built directly in the **ServiceNow Studio** environment and serves as a core portfolio piece demonstrating seamless integration between ServiceNow database configurations and **Git version control**.

---

## ✨ Features
*   **Employee Preference Engine:** Capture personalized selections for T-shirt sizes, gourmet chocolates, wine preferences, and warm winter beverages.
*   **Dynamic UI Policies:** Built-in conditional logic that automatically adapts the form interface based on the user's choices (e.g., dynamically adjusting layout options for non-alcoholic preferences).
*   **Fulfillment Pipeline:** A structured tracking lifecycle from `Requested` to `Packing`, `Shipped`, and `Delivered`.

---

## 🛠️ Architecture & Data Model

The application leverages a single core table (`x_snc_december_hamper_request`) configured with normalized relationships and choice lists:

*   **Employee:** Reference to the core ServiceNow User directory (`sys_user`).
*   **T-Shirt Size:** Choice List *(S, M, L, XL, XXL, No T-Shirt)*
*   **Chocolate Flavor:** Choice List *(Creamy Milk, Dark Sea Salt, White Raspberry, Vegan Hazelnut)*
*   **Wine Selection:** Choice List *(Red Cabernet, White Chardonnay, Sparkling Rosé, Non-Alcoholic Cider)*
*   **Warm Beverage Choice:** Choice List *(Organic Coffee Beans, Premium Tea Blend, Artisan Hot Chocolate)*
*   **Delivery Status:** Choice List *(Requested, Packing, Shipped, Delivered)*

---

## 📈 Git Version Control Workflow
This repository follows standard software development lifecycle (SDLC) best practices. The application's XML metadata structures were tracked incrementally using structured Git commit conventions:

1.  `feat: establish data model for December gift hamper preferences` — Initial table creation and choice-list schema layout.
2.  `ui: organize form layout for employee holiday selections` — Designing the interface structure using Form Designer.
3.  `ui: implement UI policy for conditional holiday choices` — Deploying client-side form behavior rules.
