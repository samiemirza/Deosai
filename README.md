# SensAI Website

Marketing website for **Deosai MedTech's SensAI** platform, built with Next.js (App Router), TypeScript, and Tailwind CSS.

SensAI is presented as an AI copilot for value-based healthcare, focused on:
- real-time risk capture
- RAF score optimization
- automated clinical documentation
- intelligent inbox workflows

## What This Site Contains

### Main routes
- `/` Home
- `/product` Product overview
- `/impact` Impact and outcomes
- `/about` Company, team, and advisory board

### Homepage sections (`/`)
- Hero: "AI-Powered Synthetic Medical Intelligence"
- Problem Statement: documentation overload, missed risk capture, fragmented workflows
- SensAI positioning and value proposition
- "What we offer" headline + horizontal offer cards
- CTA section with demo/team contact actions

### Product page (`/product`)
- Product intro headline
- 2x2 value grid (Effective, Scalable, Digital Immortality, Disruptive)
- Offer cards (shared section)
- Ground Framework for Care visual and explanatory copy

### Impact page (`/impact`)
- "Measurable Financial and Clinical Impact"
- key metrics timeline cards for risk capture, documentation time, inbox workload, and reimbursement impact

### About page (`/about`)
- Company mission statement
- interactive team and advisory board flip cards

## Tech Stack

- Next.js 14 (App Router)
- React 18
- TypeScript
- Tailwind CSS
- Framer Motion (impact animations)
- Emotion packages are installed in dependencies

## Local Development

### Prerequisites
- Node.js 18+ recommended
- npm

### Install
```bash
npm install
```

### Run dev server
```bash
npm run dev
```

Open `http://localhost:3000`.

### Production build
```bash
npm run build
npm run start
```

## Deployment Notes

The project is configured for **static export** in `next.config.js`:
- `output: "export"`
- `images.unoptimized: true`

Running `npm run build` generates static output (e.g. in `out/`) suitable for static hosting.

## Project Structure

```text
app/
  page.tsx            # Home
  product/page.tsx    # Product route
  impact/page.tsx     # Impact route
  about/page.tsx      # About route
  layout.tsx          # Global layout (Navbar + Footer)
  globals.css         # Tailwind utilities and shared styles

components/
  Hero.tsx
  Problems.tsx
  GetApp.tsx
  Guide.tsx
  Camp.tsx
  Partner.tsx
  ProdIntro.tsx
  Value.tsx
  Framework.tsx
  Traction.tsx
  About.tsx
  Team.tsx
  Navbar.tsx
  Footer.tsx

constants/
  index.ts            # Nav and footer config
```
