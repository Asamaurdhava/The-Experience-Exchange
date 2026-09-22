# The Experience Exchange

ASU's student-run skill bank. **You never name your own skills. Someone else does it first.**

A website and working prototype built for the Principled Innovation Academy challenge:
*How might we help students recognize, reflect on, and communicate the value of the experiences they gain through work, learning, and life so they can confidently tell their story?*

## What's inside

A single self-contained page (`index.html`) with:

- **Landing sections:** the problem (listening-session quotes, NACE gap), how the bank works, why it's new, Principled Innovation, and how to join
- **Working prototype**, following sample member Maya:
  1. **Anti-Resume:** an appraiser taps Invisible Work cards and the page reads the story back as strengths, with drafted resume bullets
  2. **The Vault:** a Friday text-style deposit with a follow-up question, a skill staircase chart, and a Vault statement
  3. **Ticker & Heists:** a skill-trading board with matching, plus 72-hour campus Heists that issue a signed Skill Receipt
  4. **Market Day:** an auto-built pitch card (Context, Action, Result, Reflection), a 60-second timer with a bell, and a listener scorecard

All member data, campus clients, and signatures are samples.

## Run it

No build step and no dependencies. Open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

- **GitHub Pages:** push to a repo, then Settings → Pages → deploy from the `main` branch, root folder.
- **Netlify / Vercel:** drag and drop the folder, or import the repo with no build command.

## Tech

- Plain HTML, CSS, and vanilla JavaScript in one file
- Fonts from Google Fonts: Bricolage Grotesque, IBM Plex Sans, IBM Plex Mono
- Light and dark themes via `prefers-color-scheme`
- Responsive down to phone width; respects `prefers-reduced-motion`
- The only stored state is the last-opened prototype step, in `localStorage`

## Prototype evidence

The `evidence/` folder holds a companion page (`evidence/index.html`), a 52-second video walkthrough (`evidence/walkthrough.mp4`), and 10 screenshots of every step on desktop and phone (`evidence/shots/`).

## Structure

```
experience-exchange/
├── index.html          # the whole site and prototype
├── evidence/
│   ├── index.html      # prototype evidence page
│   ├── walkthrough.mp4 # 52-second video walkthrough
│   └── shots/          # 10 screenshots
└── README.md
```
