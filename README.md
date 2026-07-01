# Akata — AI-Powered Smart Hiring for Campus Recruitment

> AI handles initial screening efficiently, but the final decision is always with humans. A win-win platform — better shortlists for recruiters, real improvement feedback for students.

Akata is an AI-powered smart hiring platform built for campus recruitment. It solves two problems at once: recruiters miss good candidates due to poor matching, and students get unfair opportunities with no feedback to improve. Akata uses vector-based semantic matching, adaptive testing, interactive artifacts, AI avatar interviews, and structured rubric scoring to deliver a fairer, deeper, faster hiring pipeline.

## Live Preview

The site is a single-page marketing landing page built with Next.js 16, motion animations, HLS.js video background, and a dark-mode design system.

## Features Showcased

- **Vector-based Semantic Matching** — Sentence-Transformers + ChromaDB
- **Adaptive Testing** — Difficulty self-adjusts based on candidate performance
- **Interactive Artifacts** — Dynamic HTML components (Mermaid diagrams, code editors, comparison tables) generated per candidate
- **Natural AI Avatar Interview** — Lifelike avatar with lip sync and behavioral analysis
- **Professional Hiring Rubric** — Weighted scoring across 5 categories (Technical 35%, Project 25%, Communication 20%, Adaptability 10%, Behavioral 10%)
- **Candidate Feedback System** — Personalized improvement reports
- **Multi-Agent System** — Test Agent + Web Search Agent + Artifact Generator
- **Hybrid Architecture** — Local inference (Ollama, Whisper) + cloud coordination where it earns its keep

## Tech Stack

- **Framework:** Next.js 16 with App Router
- **Language:** TypeScript 5
- **Styling:** Tailwind CSS 4 + shadcn/ui (New York)
- **Animations:** `motion` (Framer Motion)
- **Video:** `hls.js` for streaming background
- **Icons:** `lucide-react`
- **Fonts:** Instrument Sans + Instrument Serif (Google Fonts)

## Project Structure

```
src/
├── app/
│   ├── layout.tsx          # Root layout, dark theme, Akata metadata
│   ├── page.tsx            # Composes all sections
│   └── globals.css         # Tailwind + Instrument fonts + custom utilities
└── components/
    ├── akata/              # All Akata-specific sections
    │   ├── navbar.tsx
    │   ├── hero.tsx        # HLS video background, motion animations
    │   ├── how-it-works.tsx
    │   ├── features.tsx
    │   ├── artifacts.tsx   # Interactive artifact mockup
    │   ├── stats-usp.tsx
    │   ├── tech-stack.tsx
    │   ├── rubric.tsx      # Weighted scoring visualization
    │   ├── benefits.tsx    # Tabbed: Students / Recruiters / Colleges / Overall
    │   ├── final-cta.tsx
    │   ├── footer.tsx
    │   └── coming-soon-handler.tsx  # Global toast interceptor
    └── ui/                 # shadcn/ui primitives
```

## Getting Started

```bash
# Install dependencies
bun install

# Run dev server
bun run dev

# Open http://localhost:3000
```

## Customization

- **Waitlist link:** Replace the Google Form URL in `navbar.tsx`, `hero.tsx`, `final-cta.tsx`, and `footer.tsx`
- **Colors:** Edit the palette in `globals.css` and the `#3054ff` / `#b4c0ff` constants across components
- **Sections:** Add or remove sections in `src/app/page.tsx`

## License

MIT — built for the Akata team.
