# Security+ Academy — SY0-701

A deployable, mobile-friendly React/Vite study application with daily lessons, original practice quizzes, answer explanations, three simplified PBQ labs, timed mock exam mode, and browser-local progress.

## Run locally

Requires Node.js 18+.

```bash
npm install
npm run dev
```

Open the local URL shown in your terminal (typically http://localhost:5173).

## Deploy online

**Vercel:** Push this folder to a GitHub repository, import it into Vercel, select Vite, set Build Command to `npm run build`, and Output Directory to `dist`. Deploy.

**Netlify:** Import the Git repository, use Build Command `npm run build` and Publish Directory `dist`.

**Cloudflare Pages:** Connect the repository, use Build Command `npm run build` and Build Output Directory `dist`.

No API keys or server are required for this starter app. It is a single-page application with no client-side route rewriting needed.

## Progress storage

The app stores completed lessons and quiz attempts in `localStorage` under `security-plus-academy-v1`. Data stays in the browser, does not sync across devices, and can be lost if browser storage is cleared. Export progress from the Progress page for a backup. No login system is included.

## Scope and limitations

- Starter bank: 24 unique original multiple-choice questions, 16 short lessons, 3 simplified PBQ simulations.
- The 90-question mock exam reuses questions from the starter bank; it is **not** a validated full-length readiness test. Expand the question bank with many more unique, reviewed questions before relying on mock scores.
- Questions cover all five SY0-701 domains, but this starter content is **not** exhaustive coverage of the official objectives.
- The timed mock is 90 minutes. Unanswered questions count as incorrect.
- No affiliation with CompTIA. Security+ and CompTIA are trademarks of CompTIA, Inc.

## Expand content

Edit `src/data.js` to add more lessons, questions, and PBQ scenarios. Question entries are `[prompt, [four options], correctIndex, explanation, domainIndex]`, where `correctIndex` is 0–3 and `domainIndex` is 0–4.
