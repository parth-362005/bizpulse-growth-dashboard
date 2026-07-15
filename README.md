# BizPulse — Local Business Growth Dashboard

A premium, production-quality SaaS-style dashboard for local retail businesses — built as a final-year B.Tech resume project. Includes inventory, POS billing, customers, invoices, profit analytics, AI sales prediction, GST reports, WhatsApp notifications, and employee management. 100% frontend, powered by realistic dummy data (no backend required).

## Features

- 12 fully-built pages: Login, Dashboard, Inventory, Sales (POS), Customers, Invoices, Profit Analytics, AI Sales Prediction, GST Reports, WhatsApp Notifications, Employee Management, Settings
- Light & Dark mode with a persistent theme toggle
- Fully responsive — desktop, tablet, and mobile layouts
- Collapsible sidebar, global search, notification bell, profile dropdown
- Interactive charts (Recharts): area, bar, line, pie, radial, heatmap
- Reusable component library: Button, Input, Card, Table, Modal, Badge, Avatar, Pagination, SearchBar, Dropdown, Toasts, Confirm Dialogs
- Realistic dummy data: 80 products, 32 customers, 26 invoices, 8 employees, AI forecasts, GST summaries
- Smooth animations via Framer Motion
- Forms via React Hook Form (Add Product, Add Customer, Add Employee, Login, Settings)

## Tech Stack

React 18, Vite 5, Tailwind CSS 3, React Router DOM 6, Recharts 2, Lucide React, Framer Motion, React Hook Form, Context API

## Getting Started

```bash
npm install
npm run dev
```

Open http://localhost:5173 — the login screen is pre-filled with demo credentials, just click "Sign In to Dashboard".

## Build for production

```bash
npm run build
npm run preview
```

## Project Structure

```
src/
├── components/
│   ├── ui/            Button, Input, Card, Modal, Table, Badge, Avatar, etc.
│   ├── layout/         Sidebar, Navbar
│   └── dashboard/      KpiCard, ChartCard
├── pages/               One file per route
├── layouts/             DashboardLayout (sidebar + navbar + outlet)
├── context/             ThemeContext, AppContext
├── data/                 Dummy data generators
├── utils/                format.js, seededRandom.js
├── App.jsx
├── main.jsx
└── index.css
```

## Design

Inspired by Stripe, Linear, Vercel, Notion, Clerk, and Supabase - glassmorphism accents, soft shadows, rounded corners, and an indigo/violet brand palette with Lexend + Plus Jakarta Sans typography.

## Notes

- This is a frontend-only demo — no backend, API, or real authentication. All data is generated locally with a seeded random generator so it stays consistent across reloads.
- Swap in real APIs by replacing files in `src/data/` with API calls.
