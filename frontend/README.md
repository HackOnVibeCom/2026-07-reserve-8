<div align="center">

# 💊 Expirova
### AI-Powered Smart Expiry Management System

*"Never miss an expiry date again."*

Built with ❤️ using React, Vite, Node.js, Express, MongoDB, OCR & AI

---

![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite)
![NodeJS](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js)
![Express](https://img.shields.io/badge/Express-black?style=for-the-badge&logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=jsonwebtokens)

### 🚀 Built for Hackathons • Healthcare • Smart Inventory • AI Automation

</div>

---

# 📖 Overview

Managing expiry dates manually is inefficient, error-prone, and leads to massive financial loss and medical risks.

**Expirova** is an AI-powered expiry management platform designed for hospitals, pharmacies, laboratories, warehouses, and retail businesses.

Instead of manually checking expiry dates, users simply scan products using their camera. Expirova extracts product information, stores it securely, continuously monitors expiry status, and proactively alerts users before products expire.

The platform minimizes waste, improves inventory efficiency, and helps organizations maintain compliance.

---

# 🎯 Problem Statement

Organizations handling medicines and perishable goods face several challenges:

- Manual expiry tracking
- Product wastage
- Human errors
- Missing expiry deadlines
- Inventory inefficiency
- No centralized monitoring
- Difficult batch management

Expirova automates the complete lifecycle.

---

# 💡 Solution

Expirova provides

- AI-assisted product scanning
- OCR-based expiry extraction
- Centralized inventory
- FEFO inventory management
- Real-time expiry alerts
- Smart dashboard analytics
- Organization-wide monitoring

---

# 🏗 System Architecture

```text
                   USER
                     │
                     ▼
              React + Vite Frontend
                     │
         React Router + Components
                     │
             API Service Layer
                     │
────────────── REST APIs ──────────────
                     │
             Express.js Backend
                     │
      Authentication Middleware (JWT)
                     │
        Business Logic & Validation
                     │
       OCR / AI Processing Services
                     │
               MongoDB Database
                     │
          Notification Scheduler
                     │
        Email / Dashboard Alerts
```

---

# 🎨 Frontend Architecture

```text
src
│
├── assets
├── components
│      ├── Dashboard
│      ├── Inventory
│      ├── Scanner
│      ├── Alerts
│      ├── Profile
│      ├── Navbar
│      └── UI
│
├── pages
│      ├── Home
│      ├── Scan
│      ├── Inventory
│      ├── Alerts
│      └── Profile
│
├── hooks
├── context
├── services
├── utils
├── routes
├── App.jsx
└── main.jsx
```

---

# 🚀 Complete Frontend Flow

## 1️⃣ Dashboard

The dashboard serves as the command center.

Displays

- Total Managed Items
- Expiring Soon
- Urgent Actions
- Recent Scans
- Weekly Statistics

Users can instantly

- Start AI Scan
- Add Item Manually
- View Recent Activities
- Navigate across modules

---

## 2️⃣ Smart Scanner

Users simply press

**Open Camera**

↓

Camera captures medicine package

↓

OCR extracts

- Product Name
- Batch Number
- Manufacturing Date
- Expiry Date

↓

AI validates extracted data

↓

Preview displayed

↓

User confirms

↓

Product saved into inventory

---

## 3️⃣ Inventory Management

Displays all tracked products.

Supports

- Search
- Category Filter
- Location Filter
- FEFO Sorting
- Status Filter

Every inventory card displays

- Product Name
- Batch ID
- Category
- Expiry Date
- Location
- Current Status

Status Categories

🟢 Stable

🟡 Warning

🔴 Urgent

---

## 4️⃣ Alert Management

The alert system automatically categorizes products into

Urgent

↓

Expiring Tomorrow

↓

7–14 Days Warning

↓

Safe Products

Users can

- Mark item as used
- Resolve alert
- Scan replacement
- Continue monitoring

---

## 5️⃣ Profile & Settings

Organization profile

User information

Notification preferences

Reminder timing

Security settings

Organization details

Email preferences

---

# 🔄 User Journey

```text
Open Website
      │
      ▼
Dashboard
      │
      ▼
Scan Product
      │
      ▼
OCR Reads Label
      │
      ▼
Backend Validation
      │
      ▼
Save Product
      │
      ▼
Inventory Updated
      │
      ▼
Expiry Monitoring
      │
      ▼
Notifications Generated
      │
      ▼
Dashboard Statistics Updated
```

---

# ⚙ Backend Workflow

Although this repository contains the frontend, the application communicates with a backend service responsible for all business logic.

---

## Authentication Module

User Login

↓

JWT Generated

↓

Token Stored

↓

Protected API Access

---

## Product Management

When a product is scanned

Frontend sends

```json
{
  "productName":"",
  "batchNumber":"",
  "expiryDate":"",
  "manufacturingDate":"",
  "location":"",
  "category":""
}
```

Backend

✔ validates data

✔ removes duplicates

✔ stores in MongoDB

✔ calculates expiry status

---

## OCR Pipeline

Camera Image

↓

Image Preprocessing

↓

OCR Engine

↓

Text Detection

↓

AI Parsing

↓

Structured Product Data

↓

Frontend Confirmation

---

## Expiry Engine

Whenever a product is stored

Backend calculates

```text
Remaining Days

↓

≤1 Day
Urgent

↓

≤14 Days
Warning

↓

Otherwise

Stable
```

These values automatically update the dashboard.

---

## Notification Service

Background Scheduler

↓

Checks every product

↓

Calculates remaining days

↓

Creates notification

↓

Updates alerts page

↓

(Optional)

Sends Email Notification

---

## MongoDB Collections

```text
Users

Products

Notifications

Organizations

Settings

Audit Logs
```

---

# 📦 Tech Stack

## Frontend

- React
- Vite
- React Router
- Tailwind CSS
- Axios
- React Hooks

---

## Backend

- Node.js
- Express.js
- JWT Authentication
- REST APIs
- Multer
- OCR Engine
- AI Parsing Service

---

## Database

- MongoDB
- Mongoose

---

## Deployment

Frontend

- Vercel

Backend

- Render / Railway

Database

- MongoDB Atlas

---

# ✨ Key Features

✅ Smart Camera Scanner

✅ OCR Extraction

✅ AI Product Recognition

✅ Inventory Dashboard

✅ FEFO Inventory

✅ Search & Filters

✅ Expiry Prediction

✅ Alert System

✅ Organization Management

✅ Profile Management

✅ Notification Preferences

✅ Mobile Responsive

---

# 🚀 Future Scope

- Barcode Scanner
- QR Code Detection
- AI Expiry Prediction
- Voice Assistant
- Multi Organization Support
- Analytics Dashboard
- ML Demand Forecasting
- IoT Refrigerator Monitoring
- WhatsApp Alerts
- SMS Alerts
- Offline Mode
- Cloud Sync

---

# ⚡ Installation

```bash
git clone https://github.com/yourusername/expirova-frontend.git

cd expirova-frontend

npm install

npm run dev
```

---

# 🔐 Environment Variables

```env
VITE_API_URL=

VITE_SUPABASE_URL=

VITE_SUPABASE_ANON_KEY=

VITE_AI_ENDPOINT=
```

---

# 🤝 Team Workflow

Frontend

⬇

Consumes REST APIs

⬇

Backend Processes Requests

⬇

MongoDB Stores Data

⬇

Notification Service Updates Alerts

⬇

Frontend Automatically Refreshes Dashboard

---

# 🏆 Why Expirova?

✔ Reduces medical waste

✔ Improves inventory efficiency

✔ Prevents expiry-related losses

✔ Supports hospitals and pharmacies

✔ AI-powered automation

✔ Built with scalability in mind

✔ Modern responsive UI

✔ Clean modular architecture

✔ Production-ready design

---

<div align="center">

## 🌟 "Scan Smarter. Track Better. Never Miss an Expiry."

### Made with ❤️ for Hackathons

</div>
