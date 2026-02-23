# VanLife

A React-based BaaS (Backend as a Service) application for browsing and renting camper vans. Hosts can manage their van listings, track income, and view reviews through a dedicated dashboard.

## Features

- **Browse Vans** — Filter and explore available vans by type (simple, luxury, rugged)
- **Van Details** — View pricing, descriptions, and photos for each van
- **Host Dashboard** — Manage listings, view earnings, and monitor reviews
- **Authentication** — Login system with protected host routes
- **Responsive Design** — Works across desktop and mobile devices

## Tech Stack

- **React 18** — UI library
- **React Router v6** — Nested routes, loaders, outlets
- **Firebase Firestore** — Database (BaaS)
- **MirageJS** — API mocking for development
- **Vite** — Build tool and dev server

## Login Credentials

| Email       | Password |
| ----------- | -------- |
| `b@b.com`   | `p123`   |

## Getting Started

```bash
npm install
npm run dev
```

The app will be available at `http://localhost:5173`.

## Scripts

| Command           | Description              |
| ----------------- | ------------------------ |
| `npm run dev`     | Start development server |
| `npm run build`   | Production build         |
| `npm run preview` | Preview production build |