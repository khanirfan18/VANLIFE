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

Head over to https://vitejs.dev/ to learn more about configuring vite
## About Scrimba

At Scrimba our goal is to create the best possible coding school at the cost of a gym membership! 💜
If we succeed with this, it will give anyone who wants to become a software developer a realistic shot at succeeding, regardless of where they live and the size of their wallets 🎉
The Fullstack Developer Path aims to teach you everything you need to become a Junior Developer, or you could take a deep-dive with one of our advanced courses 🚀

- [Our courses](https://scrimba.com/courses)
- [The Frontend Career Path](https://scrimba.com/fullstack-path-c0fullstack)
- [Become a Scrimba Pro member](https://scrimba.com/pricing)

Happy Coding!