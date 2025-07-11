# 🆘 EMO – Emergency Medicine Online

Live App: [https://emoa-5f7b3.web.app](https://emoa-5f7b3.web.app)

## 🧠 Overview

**EMO (Emergency Medicine Online)** is a web-based platform designed to help people quickly access emergency medicines and healthcare assistance in urgent situations. It connects patients with nearby pharmacies and medical providers in real time.

## 🎯 Problem It Solves

- Delays in getting emergency medication.
- Difficulty locating available stock near the patient.
- Lack of centralized emergency response in medicine delivery.

---

## ✅ Key Features

- 🚑 **Emergency Request System** – Users can raise instant medicine requests.
- 🏥 **Live Pharmacy Mapping** – Shows available nearby pharmacies with stock.
- 🔄 **Real-Time Status Updates** – Users are notified as the request is processed.
- 👩‍⚕️ **Admin Dashboard** – For pharmacists or hospital staff to manage incoming requests.
- 🔐 **Authentication** – Secured user login system.
- 📦 **Medicine Inventory Management** – Manage stock levels for fast decisions.

---

## 💡 Tech Stack

| Layer        | Technologies                     |
|--------------|----------------------------------|
| Frontend     | React.js, TailwindCSS            |
| Backend/API  | Firebase Functions (optional)    |
| Auth & DB    | Firebase Auth, Firestore         |
| Hosting      | Firebase Hosting                 |
| Tools        | VS Code, Git                     |

---

## 🧱 Architecture Diagram

```plaintext
                    +-------------------------+
                    |     User Browser        |
                    |  (React Web App)        |
                    +------------+------------+
                                 |
                       HTTPS Requests (REST)
                                 |
                    +------------v------------+
                    |     Firebase Hosting    |
                    +------------+------------+
                                 |
                +-----------------------------+
                |     Firebase Firestore DB   |
                | - User Profiles             |
                | - Emergency Requests        |
                | - Medicine Inventory        |
                +-----------------------------+
                                 |
                    +------------v------------+
                    |   Firebase Auth (Login) |
                    +-------------------------+
