# Get Yorked Post Studio

A single-file web app that runs the whole @get_yorked post-creation process, start to finish, in one screen. No install, no backend, no account. Open it and make a post.

## How to open it
Double-click `index.html` (opens in your browser), or serve the folder:
```
cd GetYorked-Post-Studio
python3 -m http.server 4599
# then open http://localhost:4599
```
Everything runs in the browser. Your drafts are saved in the browser (localStorage), nothing leaves your machine.

## The full pipeline (left to right)
1. **Angle** — pick the content type. The app tells you the reach lane: outrage travels (shares, cold reach), warmth stays inside the audience unless you pair it with an amplifier.
2. **Headline** — enter the York anchor + subject + one claim, hit Generate, get on-formula variations (straight declarative, hollow-quote, "Who is", correction framing, irony marker, Meet tag-on). Live check: York-anchored + line count vs the "be like water" cap.
3. **Caption** — Draft caption builds the right hook for the type (news = numeric-staccato, entertainment = question/contrarian), adds body, CTA, source line. Word counter vs the length band.
4. **Hashtags** — curated York bank, max 5 enforced, add your own.
5. **Cover** — the real 1080x1350 4:5 cover renders live on canvas in Space Grotesk. Drop a **real photo** (never AI), position it, set the scrim. Pick a template (RTN Red, Headline Bar, Breaking, Minimal).
6. **Pre-flight** — auto-lint against the brand rules. Red items block posting.
7. **Export** — Download cover PNG (exact 1080x1350), Copy full post (caption + hashtags), Save to queue.

## What it enforces (the Get Yorked format, baked in)
- York-anchored declarative headline, one claim per cover
- Line-count "be like water" cap (news 2-4, entertainment 1-2, hard cap 5)
- Headline auto-fit with a 64px floor, body-readable sizing
- Caption length bands (carousel 60-120, single 20-50)
- Max 5 hashtags
- No em-dashes (blocks on detection)
- No AI images (real-photo reminder + check)
- **Named-accusation defamation guard** — if a post makes a wrongdoing claim, it flags the 4-gate check (retrievable record naming the person, actual charge stated as charged-not-convicted, chance to respond, stated as unproven allegation) before you post.

## The Playbook tab
The whole format spec lives inside the app (Playbook tab) so you never need this file open to remember the rules.

## Source of the rules
Distilled from the Get Yorked internal format spec (voice, headline formula, caption bands, reach patterns, and the named-accusation verification discipline).
