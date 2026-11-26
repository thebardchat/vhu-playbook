# CLAUDE.md — VHDU VampireHunters Playbook Site

## What this is
A public GitHub Pages site for the **<VHDU> VampireHunters** alliance in *Last Z: Survival Shooter*, State 788. Alliance members read it on their phones. It holds the alliance rule, attack and defense checklists, event plans, and a place for members to leave notes and ideas.

Owner: Shane (GitHub: thebardchat, in-game name thebardchat). Alliance leader: INVICTUS Beard.
Goal: help every member play better, ethically and legally, and help Shane teach other players.

## Start here
1. Run `ls` and `git remote -v` first. Do not assume a fresh setup.
2. Read `index.html` fully before changing anything. It is the whole site right now.
3. Work on **one thing at a time**. Finish it, check it, then stop and say what is next. Do not pile on extra improvements.

## Hard rules (never break these)
- [ ] **No roster, no power numbers, no HQ levels, no player names** on the site. It is public and enemies can scout it. Alliance leader and Shane may be named only if they ask.
- [ ] **Never mention any previous alliance.** Shane does not want it mentioned anywhere.
- [ ] **Ethical and legal play only.** No hacks, generators, bots, account sharing, or "free gems" links. Link only to official game sources.
- [ ] **Do not invent game facts.** If a number or rule is unconfirmed, mark it with the TEST or VERIFY tag already used in the page. Never present a guess as fact.
- [ ] **No personal info about members.** No real names, locations, or contact details.
- [ ] **Do not publish the notes form answers** (Google Form responses) on the site without Shane approving each one.

## Voice and style
- **Simple English.** Short sentences. Many members are not native English speakers and read on small screens.
- Friendly, fun, a little bold. Vampire-hunter theme is welcome. No cursing.
- Headers, bullets, and checkboxes. Short blocks.
- Use "operators" never "drivers" if truck work ever comes up.

## Design rules
- **Colors: red, black, and gold.** Never green. (Shane's school colors are red.)
- **Mobile first.** Test at 420px wide before anything else. Then check desktop.
- Keep text large and easy to read. Buttons easy to tap.
- Keep the dark theme and the sticky top menu.
- Must work on an old phone: no heavy libraries.

## Tech rules
- **Static site only.** HTML, CSS, and plain JavaScript. No build step, no framework, no server, no paid services.
- GitHub Pages deploys from the `main` branch root. Keep `index.html` at the root.
- Splitting into more pages is fine (`/pages/*.html`, `style.css`, `app.js`). Keep one shared header, menu, and footer so pages look the same.
- Keep the three config lines near the bottom of the script (`FORM_LINK`, `FORM_EMBED`, `DISCUSSIONS`). Move them to a small `config.js` if you split the files. Shane fills these in himself.
- Checkbox state saves in the visitor's own browser (`localStorage`). Keep the try/catch around it.
- No tracking scripts, no ads, no external fonts or CDNs unless Shane approves.

## Where the facts come from
Source of truth is the Claude Project **"last-z"** (Shane's notes). Do not copy facts from memory. Ask Shane to paste or confirm updates. Key facts already on the site:
- Alliance rule: "Never farm a non-farming player or alliance. Everyone else is fair game. Expect to get farmed and expect to fight back."
- Join rule: HQ 20+. Home server: State 788.
- Alliance job: attack enemy HQs and "Tanks" (enemy marches that come out of HQs to attack us).
- Peace Day: attack no one, only plunder your selected server.
- Saturday (Alliance Duel Day 6): combat day, free teleport to the enemy server, 4 points per kill. Duel needs about 20+ members (check in game).
- Volcano War: Day 6, 12:00 Apocalypse Time for 1 hour. HQ 15+ to teleport. 2,000 personal points for ranking rewards. One guide only, so mark VERIFY.
- Apocalypse Time = Central Time + 4 hours.
- Faction counters: Wings beat Blood Rose beat Guard of Order beat Wings.

## Make it look better — first jobs (do in this order, one at a time)
1. [ ] **Hero header:** better logo-style title, subtle vampire theme (fangs, bats, moon) drawn with CSS or inline SVG. Original art only. Do not copy any game art, logos, or characters.
2. [ ] **Cards and spacing:** cleaner sections, icons for each section, better tap targets.
3. [ ] **Tables:** nicer tables for Volcano War spots and faction counters.
4. [ ] **Sticky "Attack Day" button** that jumps to the checklist.
5. [ ] **Print / screenshot friendly** version of the checklist so leaders can paste it into alliance chat.

## Expand the content — next jobs
1. [ ] **Page: New Player Start** — first 7 days in simple steps. Use only confirmed facts.
2. [ ] **Page: Heroes and Factions** — tips and counters. Mark unconfirmed items.
3. [ ] **Page: Resources and Shields** — when to shield, what to protect.
4. [ ] **Page: Events Calendar** — weekly Alliance Duel themes Mon–Sat, Volcano War timeline. Mark VERIFY where needed.
5. [ ] **Page: Glossary** — plain-English meanings (HQ, rally, plunder, farm, Tanks, F1, etc.).
6. [ ] **Page: Lessons Learned** — a changelog of what members tested and found. Only add items marked as confirmed in game.
7. [ ] **FAQ** built from the questions members send in the notes box.

## Notes and suggestions box
- The "Your Ideas" section links to a Google Form (works with no account) and GitHub Discussions (needs an account).
- Do not build a custom backend. If members need a no-login option, use the form.
- When Shane pastes member notes in, sort them into: **Confirmed in game**, **Needs a test**, **Opinion/Idea**. Only the first group becomes site content.

## Before you say it is done
- [ ] Open `index.html` in a browser at 420px wide. Take a screenshot and look at it.
- [ ] Click every menu link. No broken anchors.
- [ ] Search the files for player names, power numbers, and any old-alliance name. There must be none.
- [ ] Check every checkbox saves and the Clear button resets them.
- [ ] No console errors.
- [ ] Update the "Last updated" date in the footer.

## Git
- Small commits with plain messages ("Add Peace Day section").
- **If there is a merge conflict, state which version you are keeping and why before running the command.**
- Never commit passwords, tokens, or the Google Form edit link.
- Push to `main`. GitHub Pages republishes in about a minute.

## How to report back to Shane
- Say what changed in 2 to 4 short lines.
- Say what you checked.
- Say the one next step. Do not list ten ideas.
- If you do not know something, say so plainly.
