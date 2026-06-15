# Relocation Companion — Prototype

> A prototype built to visualize, validate, and feel out the real product before writing a single line of backend code.

🔗 **Prototype (this repo):** single `index.html`, no build step, open and explore  
🔗 **Live Product:** [relocation-companion-rouge.vercel.app](https://relocation-companion-rouge.vercel.app)  
🔗 **Product Source:** [github.com/BetterVersionOfPuja/relocation-companion](https://github.com/BetterVersionOfPuja/relocation-companion)

---

> [!WARNING]
> **This is a rough sketch, not a spec.**
> The UI, features, flows, data, and copy in this prototype are placeholder-level thinking — good enough to validate an idea, not good enough to hold me to. The real product will look different, work differently, and make different decisions. Don't treat anything in here as a commitment to how the final product will be built.

---

## Why this prototype exists

Relocation is one of the biggest decisions a person can make — and the research process is a mess. Dozens of tabs. Fragmented information. No single place that answers: *Can I actually afford this? What am I trading away? What do I need to do before I go?*

I wanted to build something that fixes that. But before committing to a full MERN stack, real APIs, and a production database, I needed to see it. Not wireframes. Not a Figma file. A working thing I could click through, feel the flow of, and stress-test the idea against.

So I built this prototype — entirely in one HTML file, with hardcoded data and no backend — to answer one question: **does this actually work as a product?**

The answer was yes. And now the real product is being built.

---

## What this prototype covers

A rough visual sketch of the full product vision — built to see how the ideas feel before building anything real:

- **Abroad Life Comparison** — side-by-side cost breakdown between origin and destination city
- **Budget Estimator** — salary → take-home → savings verdict
- **Visa Checklist** — document tracking and application timeline by visa type
- **Survival Translator** — essential phrases with audio for when you land
- **Offline Essentials** — hospitals, transport, grocery stores, and budget stays pre-saved per city
- **Profile & Settings** — notifications, preferences, account management

This is a thinking tool. The real product will evolve significantly from what's sketched here.

---

## What's being built next (the real product)

The prototype validated the concept. The actual [Relocation Companion](https://github.com/BetterVersionOfPuja/relocation-companion) is a full-stack MERN application, already live in early form. Here's what's been built and what's coming:

**Built so far:**
- City comparison engine — 45+ cities, 9 relocation metrics (rent, food, transport, salary, quality of life, safety, healthcare, pollution, internet)
- Saved comparisons — authenticated users can save and revisit city pairs
- Auth system — register, login, JWT + refresh tokens, protected routes, change password, delete account
- REST API with Express 5, MongoDB Atlas, Mongoose schemas, bcrypt, cookie-based sessions
- React frontend with React Router 7, Framer Motion, Tailwind CSS 4, Axios, Context API

**Coming next:**
- Live exchange rates (replacing hardcoded values)
- Real visa data by country pair
- AI-powered relocation recommendations
- Budget planner with end-to-end moving cost estimation
- Full offline mode — PWA with service worker, offline maps, offline translator
- Survival translator with real phrase sets for all destination languages
- Essential places with real geocoded data, not hardcoded SVG pins
- Deep-dive city analysis with more data sources and interactive visualizations

The vision is a product that's useful *before* you leave (comparison, budget, visa, planning) and *after* you land (offline maps, language, local essentials) — a single companion for the entire relocation journey.

---

## About the prototype stack

Everything in this repo runs in one `index.html` with zero dependencies and zero build step.

- **Chart.js 4.4** (CDN) for the budget donut chart
- **Web Speech API** for phrase audio — uses the device's built-in TTS, works offline once cached
- **Google Fonts** (Inter + Space Grotesk) loaded on first visit
- All state lives in JavaScript variables in the page — nothing is sent anywhere

To run it: clone the repo, open `index.html` in any browser.

```bash
git clone https://github.com/BetterVersionOfPuja/relocation-companion-prototype.git
cd relocation-companion-prototype
open index.html
```

---

## The real product tech stack

For reference — what the actual product is built with:

| Layer | Tech |
|---|---|
| Frontend | React.js, React Router, Tailwind CSS, Framer Motion, Axios, Context API |
| Backend | Node.js, Express.js, REST API |
| Database | MongoDB Atlas, Mongoose |
| Auth | JWT, bcrypt, HTTP-only cookies |
| Deployment | Vercel (frontend), Render (backend), MongoDB Atlas (DB) |

---

## About

**Puja Kumari** — Software Engineer, Full Stack Developer, building products that solve real problems for real people.

- GitHub: [github.com/BetterVersionOfPuja](https://github.com/BetterVersionOfPuja)
- LinkedIn: [linkedin.com/in/betterversionofpuja](https://linkedin.com/in/betterversionofpuja)
- X: [x.com/pujakumaricodes](https://x.com/pujakumaricodes)

---

*This prototype is a design and UX validation artifact. The real product is at [relocation-companion-rouge.vercel.app](https://relocation-companion-rouge.vercel.app).*
