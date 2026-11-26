# 🌾 Harvest Bridge

### Bridging Farmers and Buyers Through Smarter Agricultural Trade

Harvest Bridge is a digital agricultural marketplace designed to help farmers connect directly with potential buyers, reduce post-harvest losses, and make more informed selling decisions.

The platform focuses on helping farmers sell perishable agricultural produce before it loses value by highlighting urgency, providing market-price references, and facilitating direct connections between farmers and buyers.

---

## 🚨 Problem Statement

Farmers often face challenges when selling perishable agricultural produce:

- **Post-harvest losses:** Crops may spoil before farmers find suitable buyers.
- **Limited market access:** Farmers may depend on intermediaries to reach buyers.
- **Price uncertainty:** Farmers may lack reliable information about prevailing market prices.
- **Time-sensitive selling:** Perishable crops require quick decisions and timely sales.
- **Market inefficiency:** Farmers and buyers may struggle to discover each other efficiently.

These challenges can result in financial losses, wasted agricultural produce, and reduced income for farmers.

---

## 💡 Our Solution

Harvest Bridge provides a digital platform where farmers can list their agricultural produce and connect with potential buyers.

The platform emphasizes **urgency-based crop discovery**, helping users identify produce that needs attention sooner while improving transparency through market-price references.

Rather than replacing traditional agricultural markets or mandis, Harvest Bridge aims to complement existing market systems by providing farmers with an additional channel to discover buyers and make informed decisions.

---

## ✨ Key Features

### 👨‍🌾 Farmer Marketplace

- Create and manage crop listings.
- Add crop details such as name, quantity, price, location, and availability.
- Make agricultural produce visible to potential buyers.
- Manage listed products through the platform.

### 🛒 Buyer Discovery

- Browse available agricultural produce.
- Explore crop listings from different farmers.
- View important crop information.
- Connect with farmers regarding available produce.

### ⏳ Crop Urgency Prioritization

- Highlight crops based on estimated urgency.
- Identify produce that may require faster selling.
- Help buyers discover time-sensitive agricultural products.
- Prioritize urgent listings to improve visibility.

### 📊 Market Price Reference

- Display reference market prices for agricultural produce.
- Help farmers compare their selling prices with available market references.
- Improve price awareness and transparency.

> Market-price references are intended to support decision-making and should not be considered guaranteed real-time market prices.

### 🤝 Direct Farmer–Buyer Connection

- Reduce unnecessary barriers between farmers and buyers.
- Enable buyers to discover produce directly from farmers.
- Facilitate communication regarding crop availability and transactions.

### 🌱 Reducing Post-Harvest Waste

Harvest Bridge aims to reduce avoidable crop spoilage by making time-sensitive produce easier to discover and helping farmers reach potential buyers sooner.

---

## 🏗️ System Architecture

Harvest Bridge follows a web application architecture consisting of a frontend interface and a backend application.

```text
                  ┌──────────────────────┐
                  │       Users          │
                  │ Farmers & Buyers     │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │      Frontend        │
                  │ React + Vite         │
                  │ User Interface       │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │      Backend         │
                  │ Python + FastAPI     │
                  │ Application APIs     │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │     Database         │
                  │ Data Management      │
                  │ Crop Listings        │
                  └──────────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend

- React
- Vite
- JavaScript
- HTML5
- CSS3

### Backend

- Python
- FastAPI

### Database

- SQLite
- SQLAlchemy

### Development & Deployment

- Git
- GitHub
- Docker
- Docker Compose

---

## 📁 Project Structure

```text
TitanCore/
│
├── Harvest_Bridge_Complete-main/
│   └── Harvest_Bridge_Complete-main/
│       │
│       ├── backend/
│       │   ├── Application logic
│       │   ├── API endpoints
│       │   └── Backend configuration
│       │
│       ├── frontend/
│       │   ├── src/
│       │   │   ├── App.jsx
│       │   │   ├── main.jsx
│       │   │   ├── styles.css
│       │   │   ├── translations.js
│       │   │   └── services/
│       │   │       └── api.js
│       │   │
│       │   ├── package.json
│       │   ├── package-lock.json
│       │   └── vite.config.js
│       │
│       ├── docs/
│       │
│       ├── .env.example
│       ├── .gitignore
│       ├── Dockerfile
│       ├── docker-compose.yml
│       └── README.md
│
└── README.md
```

---

## ⚙️ Getting Started

Follow these instructions to run Harvest Bridge locally.

### Prerequisites

Make sure you have the following installed:

- [Git](https://git-scm.com/)
- [Python](https://www.python.org/)
- [Node.js](https://nodejs.org/)
- npm
- Docker *(optional, for containerized deployment)*

---

### 1. Clone the Repository

```bash
git clone https://github.com/Prajwal291/Titancore.git
```

Navigate into the repository:

```bash
cd Titancore
```

---

### 2. Navigate to the Project Directory

```bash
cd Harvest_Bridge_Complete-main/Harvest_Bridge_Complete-main
```

---

### 3. Configure Environment Variables

Create your environment file using the provided example:

```bash
cp .env.example .env
```

On Windows Command Prompt:

```cmd
copy .env.example .env
```

Configure the required environment variables according to the project setup.

**Never commit your actual `.env` file or expose secrets, credentials, or API keys publicly.**

---

### 4. Run the Frontend

Navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL displayed in your terminal, typically:

```text
http://localhost:5173
```

---

### 5. Run the Backend

Navigate to the backend directory:

```bash
cd ../backend
```

Create a Python virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment.

**Windows:**

```cmd
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

Install the backend dependencies using the dependency file provided in the backend directory.

Start the FastAPI application using the project's configured entry point.

The FastAPI documentation, when enabled, can typically be accessed through:

```text
http://localhost:8000/docs
```

---

## 🐳 Running with Docker

Harvest Bridge includes Docker configuration for containerized execution.

From the project root directory:

```bash
docker compose up --build
```

To stop the application:

```bash
docker compose down
```

---

## 🔄 How Harvest Bridge Works

### Step 1 — Farmer Lists Produce

Farmers create listings containing relevant details about their agricultural produce.

### Step 2 — Listings Become Discoverable

The listed produce becomes available for buyers to browse through the marketplace.

### Step 3 — Urgency Helps Prioritize Crops

Time-sensitive produce can receive higher visibility based on its estimated urgency.

### Step 4 — Buyers Discover Produce

Buyers browse available agricultural products and explore listings that match their requirements.

### Step 5 — Farmer and Buyer Connect

Interested buyers can contact farmers to discuss availability, quantity, price, and potential transactions.

### Step 6 — Better Selling Decisions

Market-price references help farmers make more informed decisions about their produce.

---

## 🎯 Our Impact

Harvest Bridge aims to contribute to:

- 🌾 Reduced post-harvest agricultural waste
- 💰 Improved selling opportunities for farmers
- 🤝 Better farmer–buyer connectivity
- 📊 Increased price transparency
- ⚡ Faster discovery of time-sensitive crops
- 🌱 More efficient agricultural trade

---

## 🔮 Future Scope

Potential future improvements include:

- AI-powered crop demand prediction
- Real-time mandi price integrations
- Crop spoilage prediction using environmental and crop data
- Smart buyer recommendations
- Location-based buyer discovery
- Notification system for urgent crop listings
- Farmer analytics and insights dashboard
- Multilingual support
- Secure transaction and payment integration
- Mobile application for farmers
- Weather-based agricultural insights

---

## 👥 Team TitanCore

Built with teamwork, innovation, and a shared goal of solving real-world agricultural challenges.

| Team Member | Role |
|---|---|
| **Prajwal L** | Database, Integration & Project Coordination |
| **Hemanth** | Backend Development |
| **Siddesh** | Frontend Development |
| **Chethan** | Features, Testing & Quality Assurance |

---

## 🏆 Hackathon Project

**Project Name:** Harvest Bridge  
**Team Name:** TitanCore  
**Category:** Agriculture / AgriTech / Social Impact  
**Focus:** Reducing post-harvest losses and improving farmer–buyer connectivity

---

## 🤝 Contributing

Contributions, suggestions, and feedback are welcome.

If you would like to contribute:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Push your branch.
6. Submit a Pull
