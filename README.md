<div align="center">

# 🚐 VanLife

**A modern van rental marketplace built with React**

[![React](https://img.shields.io/badge/React-18.2.0-61DAFB?style=flat-square&logo=react&logoColor=white)](https://reactjs.org/)
[![React Router](https://img.shields.io/badge/React_Router-6.4.3-CA4245?style=flat-square&logo=react-router&logoColor=white)](https://reactrouter.com/)
[![Firebase](https://img.shields.io/badge/Firebase-Firestore-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Vite](https://img.shields.io/badge/Vite-Latest-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![MirageJS](https://img.shields.io/badge/MirageJS-0.1.46-1E8449?style=flat-square)](https://miragejs.com/)

[Features](#-features) • [Tech Stack](#-tech-stack) • [Getting Started](#-getting-started) • [Project Structure](#-project-structure)

</div>

---

## 📖 About

VanLife is a React-based van rental marketplace with BaaS (Backend-as-a-Service) integration. Users can browse available vans, filter by category, and view detailed listings. Van owners (hosts) have access to a protected dashboard to manage their listings, track income, and monitor reviews.

This project showcases advanced React patterns including nested routing, protected routes, search parameters, and BaaS integration with Firebase Firestore.

---

## ✨ Features

**For Travelers:**
- Browse all available vans with filtering (Simple, Luxury, Rugged)
- View detailed van information with pricing
- Persistent search state across navigation

**For Hosts (Protected):**
- Dashboard with earnings overview and review scores
- Income tracking with transaction history
- Van management with tabbed navigation (Details, Pricing, Photos)
- Review monitoring system

**Core:**
- Authentication with protected routes
- Nested layouts with React Router v6
- Real-time data from Firebase Firestore
- Mock API server with MirageJS for development

---

## 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| **Frontend** | React 18, React Router 6, React Icons |
| **Database** | Firebase Firestore |
| **Mock Server** | MirageJS |
| **Build Tool** | Vite |
| **Styling** | Vanilla CSS |

---

## 🚀 Getting Started

### Prerequisites

- Node.js 16+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/vanlife.git
cd vanlife

# Install dependencies
npm install

# Start development server
npm run dev
```

The app will be available at `http://localhost:5173`

### Test Credentials

```
Email: b@b.com
Password: p123
```

---

## 📁 Project Structure

```
├── api.js                 # Firebase Firestore API functions
├── server.js              # MirageJS mock server configuration
├── index.jsx              # App entry point & route definitions
├── index.css              # Global styles
│
├── components/
│   ├── AuthRequired.jsx   # Protected route wrapper
│   ├── Header.jsx         # Navigation header
│   ├── Footer.jsx         # Site footer
│   ├── Layout.jsx         # Main layout wrapper
│   └── HostLayout.jsx     # Host dashboard layout
│
└── pages/
    ├── Home.jsx           # Landing page
    ├── About.jsx          # About page
    ├── Login.jsx          # Authentication
    ├── NotFound.jsx       # 404 page
    │
    ├── Vans/
    │   ├── Vans.jsx       # Van listing with filters
    │   └── VanDetail.jsx  # Individual van page
    │
    └── Host/
        ├── Dashboard.jsx      # Host overview
        ├── Income.jsx         # Earnings & transactions
        ├── Reviews.jsx        # Guest reviews
        ├── HostVans.jsx       # Manage listings
        ├── HostVanDetail.jsx  # Van management
        ├── HostVanInfo.jsx    # Van details tab
        ├── HostVanPricing.jsx # Pricing tab
        └── HostVanPhotos.jsx  # Photos tab
```

---

## 🗺 Routes

| Route | Access | Description |
|-------|--------|-------------|
| `/` | Public | Landing page |
| `/about` | Public | About page |
| `/vans` | Public | Browse all vans |
| `/vans/:id` | Public | Van details |
| `/login` | Public | Authentication |
| `/host` | Protected | Host dashboard |
| `/host/income` | Protected | Income tracking |
| `/host/reviews` | Protected | Review management |
| `/host/vans` | Protected | Manage listings |
| `/host/vans/:id/*` | Protected | Van management tabs |

---

## 🔧 API Integration

### Firebase Firestore

The app uses Firebase Firestore for persistent data storage:

```javascript
// api.js - Key functions
getVans()      // Fetch all vans
getVan(id)     // Fetch single van
getHostVans()  // Fetch host's vans (filtered by hostId)
loginUser()    // Authentication
```

### MirageJS Mock Server

For local development, MirageJS provides a mock REST API:

- `GET /api/vans` - All vans
- `GET /api/vans/:id` - Single van
- `GET /api/host/vans` - Host's vans
- `POST /api/login` - Authentication

The mock server includes 6 pre-seeded vans and test user data.

---

## 🔐 Authentication Flow

1. User attempts to access `/host/*` routes
2. `AuthRequired` component checks localStorage for auth status
3. Unauthenticated users redirect to `/login` with return path
4. After login, users return to their original destination

---

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |

---

## 📄 License

This project is open source under the [MIT License](LICENSE).

---

<div align="center">

**Built with ❤️ using React**

</div>
