# Next.js Dashboard

A financial dashboard application built with the Next.js App Router. It lets you manage invoices and customers, view revenue charts, and sign in with authentication. This project is based on the official [Next.js App Router Course](https://nextjs.org/learn).

## Live Demo

**URL:** [https://nextjs-dashboard-kappa-six-34.vercel.app/](https://nextjs-dashboard-kappa-six-34.vercel.app/)

Log in with the demo account:

- **Email:** `user@nextmail.com`
- **Password:** `123456`

## Features

- **Dashboard overview** with revenue chart, latest invoices, and summary cards
- **Invoices** management with create, edit, delete, search, and pagination
- **Customers** listing
- **Authentication** powered by NextAuth.js
- **Server Components & Server Actions** for data fetching and mutations
- **Responsive UI** styled with Tailwind CSS

## Tech Stack

- [Next.js](https://nextjs.org/) (App Router)
- [React](https://react.dev/) & TypeScript
- [Tailwind CSS](https://tailwindcss.com/)
- [PostgreSQL](https://www.postgresql.org/) via the `postgres` client
- [NextAuth.js](https://authjs.dev/) for authentication
- [Zod](https://zod.dev/) for validation

## Getting Started

### Prerequisites

- Node.js 18+
- A PostgreSQL database
- [pnpm](https://pnpm.io/) (recommended)

### Installation

```bash
pnpm install
```

### Environment Variables

Create a `.env` file in the project root:

```bash
POSTGRES_URL=your_postgres_connection_string
AUTH_SECRET=your_auth_secret
```

### Development

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Scripts

| Command | Description |
| --- | --- |
| `pnpm dev` | Start the development server (Turbopack) |
| `pnpm build` | Build for production |
| `pnpm start` | Start the production server |
| `pnpm lint` | Run ESLint |

## Project Structure

```
app/
├── dashboard/    # Dashboard pages (overview, invoices, customers)
├── login/        # Login page
├── ui/           # Reusable UI components
├── lib/          # Data fetching, actions, and definitions
└── layout.tsx    # Root layout
```

## License

This project is for learning purposes, based on the Next.js Learn course.
