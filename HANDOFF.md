# GitHub Profile README — Handoff

Repo: https://github.com/arnavpant/arnavpant (public, default branch `main`)
Local: `C:\Users\Arnav\Desktop\Personal Projects\github-readme\`

## Status: profile README is LIVE and rendering correctly
- Confirmed via screenshot — banner, typing tagline, badges, code block all render on https://github.com/arnavpant
- "Share to profile" fix worked (was stuck due to master→main rename)

## IMMEDIATE TODO — uncommitted local changes, need push
Two edits made to `README.md` but **not yet committed/pushed**:
1. Wrapped the typing-SVG + LinkedIn/Portfolio badges in `<div align="center">...</div>` (was left-aligned, user wants centered like the reference profile)
2. Added a new `![Open to Work](...)` shields.io badge to that centered row — orange/black, text "Open to Work · Full-Stack / Backend · Available Jun 2026" — moved the "open to roles" signal from the bottom "Currently" section to the top (user's request: "shud the job stuff not be at the top")
3. Trimmed the now-redundant "📍 Open to..." line from the "Currently" section near the bottom

**To finish: commit + push these.**
```bash
R="/c/Users/Arnav/Desktop/Personal Projects/github-readme"
git -C "$R" add -A
git -C "$R" -c user.name="arnavpant" -c user.email="arnavpant27@gmail.com" commit -q -m "Center hero section, surface Open to Work badge at top"
git -C "$R" push -q origin main
```
Then hard-refresh https://github.com/arnavpant and check:
- Typing tagline + LinkedIn/Portfolio/Open-to-Work badges are centered as a group
- "Open to Work" badge renders correctly (long text in shields.io badge — verify it doesn't look cramped/cut off; if so, shorten to "Open to Work · Full-Stack/Backend")

## Current README structure (top to bottom)
1. Banner SVG (assets/banner-light.svg / banner-dark.svg) — "ARNAV PANT" big bold text, orange left bar
2. Centered: typing-SVG tagline (cycles 4 lines) + LinkedIn badge + Portfolio badge + Open to Work badge
3. `const arnav = {...}` TS code block (engineer-object, unique element)
4. Intro paragraph
5. Impact badges (40K+ users, 46+ APIs, <50ms latency, 150K+ jobs) — for-the-badge style
6. Stack — categorized inline-code pills (Languages / AI-LLM / Frameworks / Infra & Data), pulled from resume
7. Experience timeline table (Finnimo, VT research, Al Ansari, Altius x2)
8. 3 project sections (Finnimo, Ouroboros w/ collapsible Mermaid diagram, WebCat)
9. "Currently" section (focus + contact pointer)
10. Email image (assets/email-light.svg / email-dark.svg) — anti-scraping, image not plaintext

## Other open items (lower priority, from original brief)
- [ ] **Pin repos manually** on https://github.com/arnavpant — "Customize your pins" → check `Ouroboros` + `Personal-Portfolio`. Do NOT pin `gemini-voyager` (it's a fork)
- [ ] Confirm LinkedIn handle `linkedin.com/in/arnavpant` is correct (not yet verified by user)
- [x] Ouroboros repo description updated (done)
- [x] Email scraper protection (done — SVG image)
- [x] Activity graph removed, replaced with "Currently" section (done)

## Useful context
- Palette: monochrome black/white + orange `#FF5C00` accent (light bg `#FFFFFF`/dark `#0A0A0A`)
- Resume used for Stack/Experience sections: `C:\Users\Arnav\Desktop\Resumes\latest general resume MADEAFTERGOOGLE USETHIS\ArnavPant_resume.pdf`
- Original design brief (mostly superseded by this session's changes): `C:\Users\Arnav\Desktop\Personal Projects\job-serch\github-design-prompt.md`
- gh CLI authenticated as `arnavpant`, repo perms confirmed (repo, read:org scopes)
