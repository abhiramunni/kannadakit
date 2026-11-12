# KannadaKit — Speak Bengaluru Like a Local

A pocket Kannada phrasebook for life in Bengaluru. 58 everyday phrases across 6 situations — polite essentials, auto & travel, food & darshini, shopping & bargaining, home & landlord, emergency — plus Kannada numbers 1–100, a pronunciation guide, and a 10-round practice quiz.

## What it does

- **Phrase deck** — every phrase shows the Kannada script, a simple transliteration, the English meaning, and a plain-words usage tip. Tap the speaker to hear it spoken (device Kannada voice via Speech Synthesis, `kn-IN`).
- **Search + category chips** — filter by situation, or search by English, transliteration or Kannada.
- **Star & learn** — star the phrases you need today, mark phrases learned, and track progress (ring in the header + sticky bottom bar). All saved in `localStorage`.
- **Numbers strip** — 1–10, 20, 50, 100 with tap-to-hear, for bargaining and fares.
- **Practice quiz** — 10 rounds in “Read it” or “Hear it” mode, with score, streak, dots, and a persistent best score.
- **How to say it** — 6 pronunciation rules (long vowels, retroflex letters, the magic word *swalpa*…).
- **When it really matters** — three emergency sentences with tap-to-hear, plus the 112 emergency number.
- **Phrase of the day** — a different phrase every day, picked by the date.
- **Cinematic intro** — full-screen golden-hour Bengaluru photo with Ken Burns drift, staggered title, progress bar, tap-to-skip (quick version on return visits), plus a 3-step onboarding coach.

## Design

Warm editorial palette (ivory paper, espresso ink, bronze/amber/gold/terracotta) with Fraunces + Inter + Noto Sans Kannada. Two AI-generated warm-editorial photos embedded in the file (Bengaluru street at golden hour; darshini filter coffee). Single self-contained `index.html` — no backend, no signup, `localStorage` only.

## Run it

Open `index.html` in any modern browser, or serve it: `python3 -m http.server` and visit `http://localhost:8000`.

## QA

`qa-test.js` — headless jsdom functional tests (deck render, search, category filter, star/learn persistence, numbers, quiz flow in both modes, intro skip, coach, erase). Run with `node qa-test.js` (jsdom required). `node --check` passes on the extracted inline script.

## Live

https://abhiramunni.github.io/kannadakit/
