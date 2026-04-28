# 🚀 Smart Supply Chain Platform

![Stars](https://img.shields.io/github/stars/WhisTech/GDG-Solution-challenge?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/WhisTech/GDG-Solution-challenge?style=for-the-badge)
![Issues](https://img.shields.io/github/issues/WhisTech/GDG-Solution-challenge?style=for-the-badge)
![License](https://img.shields.io/github/license/WhisTech/GDG-Solution-challenge?style=for-the-badge)

![CI](https://github.com/WhisTech/GDG-Solution-challenge/actions/workflows/main.yml/badge.svg)

---

## 📌 Description

A modern, AI-augmented supply chain management platform for enterprises & SMEs, featuring real-time inventory, multi-party orders, supplier management, global logistics tracking, and demand forecasting with neural networks. Built with React, Vite, Tailwind, Node.js/Express, and Sequelize ORM.

---

## ✨ Features

- 🏪 **Inventory Tracking**: Real-time warehouse stock levels and status alerts
- 📦 **Product Catalog**: Manage SKUs, categories, and pricing
- 📑 **Order Management**: Create and track B2B customer orders
- 🧾 **Purchase Orders**: Handle inbound supplier shipments and requisitions
- 🤝 **Supplier Directory**: Manage partners with ratings/contact info
- 🚚 **Logistics Map**: Live GPS map of ongoing shipments with status
- 🧠 **AI Forecast Engine**: Predict stock needs with neural forecasting
- 🔐 **Authentication**: Secure login for Admin, Supplier, Warehouse, Retailer roles
- 📊 **Dashboards**: Visualize demand, revenue, shipments, and critical KPIs

---

## 🛠️ Tech Stack

- **Frontend**: React, Vite, Tailwind CSS, Lucide icons, Axios, React Leaflet
- **Backend**: Node.js, Express, Sequelize ORM, Postgres/MySQL/SQLite
- **AI**: Google Generative AI API (Gemini)
- **CI/CD & Hosting**: Render.com, YAML pipeline
- **Other**: dotenv, JWT authentication, CORS, bcrypt

---

## 📸 Screenshots

Add your screenshots here:

- `/frontend/src/assets/hero.png`  
- `/frontend/src/assets/react.svg`, `/frontend/src/assets/vite.svg`  
> **(Place your screenshots in `./frontend/src/assets/` and reference them here!)**

---

## ⚙️ Installation

```bash
# 1. Clone the repo
git clone https://github.com/<YOUR_GITHUB>/<YOUR_REPO>.git

# 2. Install backend dependencies
cd backend
npm install

# 3. Create a .env file in ./backend (see .env.example)
cp .env.example .env

# 4. Install frontend dependencies
cd ../frontend
npm install

# 5. Run the backend server
cd ../backend
npm start

# 6. Start the frontend (in a new terminal)
cd ../frontend
npm run dev
```

---

## 🚀 Quick Start

```bash
# One-liner (from project root, for dev testing)
(cd backend && npm install && npm start) & (cd frontend && npm install && npm run dev)
```

- Backend: http://localhost:5000
- Frontend: http://localhost:5173

---

## 📂 Folder Structure

```
.
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── config/
│   │   └── ...
│   ├── .env.example
│   ├── add_stock.js
│   ├── create_users.js
│   └── seed.js
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── context/
│   │   ├── assets/
│   │   └── services/
│   ├── vite.config.js
│   └── ...
├── render.yaml
└── README.md
```

---

## 🔗 API Endpoints

### Auth
- `POST /api/auth/register` &mdash; Register new user
- `POST /api/auth/login` &mdash; Login and receive JWT

### Products / Inventory
- `GET /api/products` &mdash; List products _(auth required)_
- `POST /api/products` &mdash; Add product _(Admins/Suppliers)_
- `GET /api/inventory` &mdash; List inventory _(auth required)_
- `PUT /api/inventory/update` &mdash; Update stock _(Admin/WM/Supplier)_

### Orders & PO
- `GET/POST /api/orders` &mdash; Manage sales orders
- `GET/POST /api/purchase_orders` &mdash; Manage purchase orders

### Suppliers & Warehouses
- `GET/POST /api/suppliers`
- `GET/POST /api/warehouses`

### Shipments & Demand
- `GET /api/shipments`
- `POST /api/shipments/:id/update`
- `GET /api/demand` &mdash; Historical demand _(Admin/Supplier)_
- `POST /api/demand/predict` &mdash; AI stock forecasting

> All routes require JWT. See backend for full details.

---

## 🤝 Contributing

1. Fork the repo & create your branch (`git checkout -b feature-branch`)
2. Commit your changes (`git commit -am 'feat: add something'`)
3. Push to branch (`git push origin feature-branch`)
4. Create a Pull Request

All contributions, bug reports, and suggestions welcome!

---

## 📜 License

Distributed under the ISC License.  
See [`LICENSE`](./LICENSE) for more info.

---

> _Replace `<YOUR_GITHUB>/<YOUR_REPO>` in badge/image/clone URLs with your actual GitHub username and repo name._
