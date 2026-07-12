

<p align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0d5f94&text=Expirova&fontColor=ffffff&fontSize=55&animation=fadeIn"/>

</p>

<p align="center">

<img src="https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb"/>
<img src="https://img.shields.io/badge/Hackathon-Project-orange?style=for-the-badge"/>
<img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge"/>

</p>

<p align="center">

**AI-Powered Smart Expiry Management System**

*Scan • Track • Monitor • Prevent Waste*

</p>

---

# ✨ Features at a Glance

<table>
<tr>
<td align="center" width="25%">

### 📸 Smart OCR Scan
Extracts medicine details directly from labels using AI-powered OCR.

</td>

<td align="center" width="25%">

### 📦 Inventory Management
Organize, search, filter, and manage products using FEFO.

</td>

<td align="center" width="25%">

### 🚨 Smart Alerts
Receive proactive notifications before products expire.

</td>

<td align="center" width="25%">

### 📊 Analytics Dashboard
Monitor inventory health with real-time statistics.

</td>
</tr>
</table>

---

# ⚡ User Flow

```mermaid
flowchart LR

A[📷 Scan Product]
--> B[🤖 OCR Extraction]
--> C[🧠 AI Validation]
--> D[💾 Save Inventory]
--> E[📦 Inventory Dashboard]
--> F[⏰ Expiry Monitoring]
--> G[🚨 Smart Alerts]
```

---

# 🖼️ Application Screenshots

<table>
<tr>

<td align="center">

### 📊 Dashboard

<img src="images/dashboard.png" width="100%"/>

Real-time inventory overview, analytics, quick actions and recent scans.

</td>

<td align="center">

### 📷 Smart Scanner

<img src="images/scanner.png" width="100%"/>

Capture medicine labels and extract expiry information automatically.

</td>

</tr>

<tr>

<td align="center">

### 📦 Inventory

<img src="images/inventory.png" width="100%"/>

Search, filter, categorize and manage inventory using FEFO.

</td>

<td align="center">

### 🚨 Alerts

<img src="images/alerts.png" width="100%"/>

Automatically highlights products requiring immediate attention.

</td>

</tr>

<tr>

<td colspan="2" align="center">

### 👤 Profile & Settings

<img src="images/profile.png" width="75%"/>

Manage organization details, reminders, notification preferences and profile settings.

</td>

</tr>

</table>

---

# 🚀 System Architecture

```mermaid
flowchart TB

User

User --> React

React["⚛️ React + Vite"]

React --> API

API["🌐 REST API"]

API --> Backend

Backend["🚀 Express Server"]

Backend --> OCR

Backend --> Mongo

OCR["🤖 OCR + AI"]

Mongo["🍃 MongoDB"]

Mongo --> Notification

Notification["🔔 Notification Engine"]

Notification --> React
```

---

# 💻 Tech Stack

| Frontend | Backend | Database | AI |
|-----------|----------|-----------|-----|
| React | Node.js | MongoDB | OCR |
| Vite | Express | Mongoose | AI Parsing |
| Tailwind CSS | JWT | Atlas | OpenCV |
| React Router | REST APIs | | |

---

# 🌟 Why Expirova?

> 💊 Scan medicines in seconds.

> 🤖 AI extracts expiry details automatically.

> 📦 Smart inventory management.

> 🚨 Real-time expiry monitoring.

> 📈 Interactive dashboard.

> 📱 Responsive across all devices.

> ⚡ Built for hospitals, pharmacies and healthcare institutions.

---

# 🏆 Built For

🏥 Hospitals

💊 Pharmacies

🧪 Laboratories

🏬 Warehouses

🥫 Food Inventory

🏪 Retail Stores

---

<div align="center">

## ⭐ If you like Expirova, consider giving this repository a star!

<img src="https://capsule-render.vercel.app/api?type=waving&color=0d5f94&height=120&section=footer"/>

</div>
