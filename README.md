# 🛒 PriceRadar

### Smart Product Price Comparison Platform

**PriceRadar** is a full-stack web application that helps users discover and compare product prices through Google Shopping listings. It brings product prices, ratings, discounts, and seller links together in one place, making it easier to identify competitive deals before purchasing.

## ✨ Features

- 🔍 Search products by name or keyword
- 💰 Compare prices across available shopping listings
- 🏆 Highlight the lowest available price
- ⭐ View product ratings and reviews
- 🏷️ Explore available discounts and offers
- 📊 Visualize price comparisons
- 🔗 Visit product pages through direct links
- 📱 Responsive user interface

## 🛠️ Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | React, Vite, CSS |
| Backend | Node.js, Express.js |
| API Integration | Axios |
| Product Data | SerpApi – Google Shopping |

## 📁 Project Structure

```text
PriceRadar/
├── backend/
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── utils/
│   │   └── App.jsx
│   └── package.json
│
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js
- npm
- SerpApi API key

### 1. Clone the Repository

```bash
git clone https://github.com/GARGDAISY/PriceRadar.git
cd PriceRadar
```

### 2. Configure the Backend

```bash
cd backend
npm install
```

Create a `.env` file inside the backend folder:

```env
SERPAPI_API_KEY=your_api_key
PORT=3001
```

Start the backend:

```bash
npm run dev
```

Backend runs on:

`http://localhost:3001`

### 3. Configure the Frontend

Open a new terminal:

```bash
cd frontend
npm install
npm run dev
```

The Vite development server will display its local URL in the terminal.

## 🔑 Environment Variables

| Variable | Description |
|---|---|
| `SERPAPI_API_KEY` | API key used to retrieve Google Shopping results |
| `PORT` | Backend server port |

**Important:** Never expose your SerpApi API key in frontend code or commit your `.env` file to GitHub.

## 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/compare` | Search and compare product listings |
| GET | `/api/suggestions` | Retrieve product search suggestions |
| GET | `/health` | Check backend server status |

## 📌 Notes

- Product listings and prices are retrieved through SerpApi's Google Shopping integration.
- Prices, discounts, ratings, and availability may change.
- Results depend on the data available from the connected source.
- Always verify the final price and product details on the seller's website before purchasing.

## 🚀 Future Enhancements

- Improved product variant matching
- Historical price tracking
- Price drop notifications
- Advanced product comparison
- AI-powered shopping recommendations

## 📄 License

MIT License

---

**Built by Nandini Garg**
