# Machine Produtora — website

Website for Machine Produtora, an audiovisual production studio in Brazil. It shows the studio's services and portfolio and makes it easy to get in touch.

**Live:** https://site-produtoramachine.vercel.app

![Machine Produtora home page](public/og-image.jpg)

## Features

- **Home page:** hero, services, about, portfolio highlights and contact.
- **Portfolio page:** a dedicated `/portfolio` route with the studio's work.
- **Contact:** WhatsApp and e-mail links. The e-mail address and phone number come from environment variables.
- **Scroll handling:** `ScrollManager` scrolls smoothly to the section named in the URL hash, or back to the top when the route changes.

## Tech stack

React 18 · TypeScript · Vite · Tailwind CSS · shadcn/ui (Radix UI) · React Router · Vercel

## Getting started

Requires Node.js 18 or newer.

```bash
npm install
cp .env.example .env    # optional: set the contact e-mail and phone
npm run dev             # http://localhost:8080
```

| Variable             | Used for                         |
| -------------------- | -------------------------------- |
| `VITE_CONTACT_EMAIL` | E-mail shown in the contact area |
| `VITE_CONTACT_PHONE` | Phone shown in the contact area  |

| Script            | What it does                        |
| ----------------- | ----------------------------------- |
| `npm run dev`     | Dev server with hot reload          |
| `npm run build`   | Production build into `dist/`       |
| `npm run preview` | Serves the production build locally |
| `npm run lint`    | Runs ESLint                         |

## Project structure

```
src/
├── components/
│   ├── layout/     # SiteHeader, SiteFooter
│   ├── sections/   # Hero, Services, About, Portfolio, Contact
│   └── ui/         # shadcn/ui primitives
├── config/         # contact details
├── pages/          # HomePage, PortfolioPage, NotFoundPage
└── assets/
```

---

Built by [Heleno Matos](https://portfolio.helenomatos.com) at [Webgest Solutions](https://webgestsolutions.com.br).
