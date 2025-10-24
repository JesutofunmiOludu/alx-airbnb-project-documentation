# 🏠 Airbnb Clone Backend — Data Flow Diagram 

## 🎯 Objective
This document illustrates the **Level 1 Data Flow Diagram (DFD)** for the **Airbnb Clone Backend**.  
It shows how data moves between **actors**, **processes**, and **data stores** within the system — enabling a secure, scalable, and modular architecture.

---

## 🧩 Overview
The backend system supports three main user types:
- **Guest** — can search for properties, make bookings, and submit reviews.  
- **Host** — can list, edit, and manage their properties.  
- **Admin** — monitors overall system activities including users, bookings, and payments.

---

## 📊 Data Flow Diagram 
Below is the visual representation of the Airbnb Clone backend data flow.



![DFD Preview](./Airbnb_Backend_DFD_Level1.png)

---

## 🔁 Core Processes

### **1. Authentication & User Management**
- **Actors:** Guest / Host  
- **Input:** Registration & Login data  
- **Process:** Validates credentials and issues JWT tokens.  
- **Data Stores:** `Users`  
- **Outputs:** Authenticated user sessions and profile data.

---

### **2. Property Listings Management**
- **Actors:** Host  
- **Input:** Property details (title, price, amenities, location)  
- **Process:** Hosts can create, update, or delete property listings.  
- **Data Stores:** `Properties`  
- **Outputs:** Available property data for search and bookings.

---

### **3. Booking Management**
- **Actors:** Guest  
- **Input:** Booking requests (dates, property ID, user info)  
- **Process:** Validates availability and creates booking records.  
- **Data Stores:** `Bookings`  
- **Outputs:** Booking confirmation, status, and notifications.

---

### **4. Payment Processing**
- **Actors:** Guest / Payment Gateway  
- **Input:** Payment details (amount, booking ID, currency)  
- **Process:** Handles secure payments via third-party APIs (e.g., Stripe, PayPal).  
- **Data Stores:** `Payments`  
- **Outputs:** Payment receipts and payout confirmations to hosts.

---

### **5. Reviews & Notification System**
- **Actors:** Guest / Host  
- **Input:** Ratings, comments, or system-triggered events.  
- **Process:** Stores reviews, triggers email and in-app notifications.  
- **Data Stores:** `Reviews`, `Notifications`  
- **Outputs:** Feedback for listings and timely system alerts.

---

## 🗄️ Data Stores Summary
| Data Store | Description |
|-------------|-------------|
| **Users** | Stores guest, host, and admin profiles. |
| **Properties** | Contains property details like title, location, and pricing. |
| **Bookings** | Records all booking transactions with timestamps and statuses. |
| **Payments** | Tracks payment transactions and related booking info. |
| **Reviews** | Stores user reviews and ratings linked to specific bookings. |
| **Notifications** | Logs system and user notifications (email or in-app). |

---

## ⚙️ Tools Used
- **Draw.io (diagrams.net)** — for DFD creation  
- **Markdown (README)** — for documentation  
- **GitHub** — for version control and collaboration  

---

## 📁 File Structure

