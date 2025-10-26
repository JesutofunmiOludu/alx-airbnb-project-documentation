# 🏗️ Airbnb Clone Backend — Detailed Requirements Specification

This document outlines the detailed **backend requirements** for three key modules of the Airbnb Clone system:  
- **User Authentication**  
- **Property Management**  
- **Booking System**

Each section specifies API endpoints, input/output formats, validation rules, and performance criteria necessary for a robust backend design.

---

## 1. 🔐 User Authentication Module

### 📝 Description
This module manages user registration, login, and profile operations. It supports both **guests** and **hosts**, ensuring secure authentication and authorization using JWT.

### 📡 API Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|-----------|--------------|----------------|
| `POST` | `/api/auth/register` | Register a new user (guest or host) | ❌ |
| `POST` | `/api/auth/login` | Authenticate and generate a JWT token | ❌ |
| `GET`  | `/api/users/profile` | Retrieve current user profile | ✅ |
| `PUT`  | `/api/users/profile` | Update profile information | ✅ |
| `POST` | `/api/auth/logout` | Invalidate current session | ✅ |

---

### 🧾 Input / Output Specifications

**Register (POST /api/auth/register)**  
**Input (JSON):**
```json
{
  "full_name": "John Doe",
  "email": "john@example.com",
  "password": "P@ssw0rd!",
  "role": "host"
}
