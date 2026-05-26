# Office Sweepstake — World Cup 2026

A single-file HTML sweepstake kit for the 2026 FIFA World Cup. One admin enters
participant names, runs a randomised draw with a one-at-a-time theatrical
reveal, and downloads the results as a PDF.

## Run it

Open `index.html` in any modern browser. No build step. No server. No install.

## Deploy it

Drag `index.html` onto [drop.netlify.com](https://drop.netlify.com) — that's
the whole deploy.

## Features

- Up to 48 participants, one team per person
- Fisher-Yates randomisation (crypto-strong where available)
- One-at-a-time card reveal with flip animation
- Skip-to-end "Reveal All"
- Unallocated teams shown separately when participants < 48
- Pot calculator at £2 per entry with 50/25/15/10% payout split
- PDF export via jsPDF + jsPDF-AutoTable
- localStorage persistence across page refresh
- Light/dark theme toggle
- WCAG 2.2 AA: keyboard nav, ARIA labels, focus states, contrast
- XSS-safe (input sanitised, all rendering via `textContent`)
- CSP locked to self + jsdelivr CDN

## Data

All 48 teams from the FIFA Final Draw, 5 December 2025
([Wikipedia](https://en.wikipedia.org/wiki/2026_FIFA_World_Cup_draw)).

## Tech

- Single-file HTML, vanilla JS, embedded CSS
- jsPDF 2.5.2 + jsPDF-AutoTable 3.8.4 (jsdelivr CDN)
- No framework, no build step, no server
