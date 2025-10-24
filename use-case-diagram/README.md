# 🏠 Airbnb Clone – Use Case Diagram

## 📘 Overview
This document explains the **Use Case Diagram** for the **Airbnb Clone Backend System**.  
The diagram was created using **Draw.io** to visualize key interactions between users and the system — focusing on user registration, property listings, booking, payments, and administrative functions.



![Use Case Diagram ](/use-case-diagram.drawio.png)

---

## 🎯 Purpose
The Use Case Diagram provides a **high-level view** of how different actors (users) interact with the system.  
It helps developers, analysts, and stakeholders understand:
- The **main system functionalities**.
- The **roles** of each type of user.
- The **flow of interactions** for booking, payments, and management.

---

## 👥 Actors

| Actor | Description |
|:--|:--|
| **Guest** | A user who searches for properties, makes bookings, and leaves reviews. |
| **Host** | A user who lists properties, manages availability, and interacts with guests. |
| **Admin** | Oversees the platform, managing users, properties, and payments. |
| **Payment Gateway (External System)** | Processes secure online payments and payouts. |

---

## ⚙️ Key Use Cases

### 👤 Guest
- **Register / Login** – Create or access an account.  
- **Search Properties** – Browse available accommodations.  
- **Book Property** – Make reservations for chosen dates.  
- **Cancel Booking** – Manage existing reservations.  
- **Make Payment** – Complete transactions through a payment gateway.  
- **Leave Review** – Provide feedback after a stay.  

### 🏠 Host
- **Add / Edit / Delete Property Listing** – Manage properties on the platform.  
- **View Bookings** – Track guest reservations.  
- **Respond to Reviews** – Interact with guest feedback.  

### 👨‍💼 Admin
- **Manage Users** – Create, suspend, or delete user accounts.  
- **Manage Listings** – Approve or remove property listings.  
- **Manage Bookings** – Monitor and resolve booking issues.  
- **Monitor Payments** – Track platform-wide transactions.  

### 💳 Payment Gateway (External)
- **Process Payment** – Securely handle transactions between guests and hosts.

---

## 🧩 System Boundary
All use cases are enclosed within the **“Airbnb Clone Backend System”** boundary, representing system functionalities.  
External actors interact through specific interfaces (APIs, web portals, or dashboards).

---


---

## 🧠 Notes
- **Solid lines** represent direct interactions between an actor and a use case.  
- **Dashed lines** indicate dependency or external system communication (e.g., payment gateway).  
- The diagram aligns with **UML Use Case Diagram** standards.  

---

## 📄 File List

