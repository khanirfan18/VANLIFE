# VanLife

A full-stack React application for browsing and renting camper vans. Hosts can manage their van listings, track income, and view reviews through a dedicated dashboard.

## Features

- **Browse Vans** — Filter and explore available vans by type (simple, luxury, rugged)
- **Van Details** — View pricing, descriptions, and photos for each van
- **Host Dashboard** — Manage listings, view earnings, and monitor reviews
- **Authentication** — Login system with protected host routes
- **Responsive Design** — Works across desktop and mobile devices

## Tech Stack

- **React** with React Router v6 (nested routes, loaders, outlets)
- **MirageJS** for API mocking
- **Vite** for fast development and builds

## Getting Started

```bash
npm install
npm run dev
```

The app will be available at `http://localhost:5173`.

## Project Structure

```
├── api.js                  # API utility functions
├── server.js               # MirageJS mock server
├── index.jsx               # App entry with routes
├── components/             # Shared components (Header, Footer, Layout)
├── pages/
│   ├── Home.jsx
│   ├── About.jsx
│   ├── Login.jsx
│   ├── Vans/               # Public van browsing
│   └── Host/               # Host dashboard & van management
└── assets/images/          # Static images
```

## Scripts

| Command           | Description              |
| ----------------- | ------------------------ |
| `npm run dev`     | Start development server |
| `npm run build`   | Production build         |
| `npm run preview` | Preview production build |

Happy Coding!