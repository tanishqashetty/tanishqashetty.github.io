# Spark ⚡ — Content Concept Generator

> AI-powered concept generator for short-form creators — decide what to make before you open the camera.

Supports **YouTube Shorts · TikTok · Instagram Reels**

## What it is

Spark fills the pre-creation inspiration gap. Most AI tools help you *edit* or *produce* content. Spark helps you figure out *what* to make — with platform-native hooks, narrative arcs, CTAs, and cover frame concepts.

## Stack

- React 18 + Vite
- Claude API (`claude-sonnet-4-20250514`)
- No backend — direct browser API calls

## Setup

```bash
git clone https://github.com/[your-username]/spark
cd spark
npm install
npm run dev
```

Add your Claude API key to the fetch headers in `src/App.jsx`:

```js
headers: {
  "Content-Type": "application/json",
  "x-api-key": "YOUR_KEY_HERE",
  "anthropic-version": "2023-06-01",
  "anthropic-dangerous-direct-browser-access": "true",
}
```

For production, use `import.meta.env.VITE_ANTHROPIC_API_KEY` with a `.env` file.

## Deploy

```bash
npm run build
# Deploy /dist to Vercel or Netlify
```

## Portfolio docs

- [`BRIEF.md`](./BRIEF.md) — one-page product brief
- [`CASE_STUDY.md`](./CASE_STUDY.md) — full case study

## What this demonstrates

- Multi-platform product thinking (not just YouTube)
- Creator-stage-aware outputs
- Metric framework for GenAI adoption in creative tools
- Roadmap gated on metric thresholds, not calendar dates

---

*Independent portfolio project. Not affiliated with YouTube, TikTok, or Meta.*
