# Hometown Comeback: handoff

> Last checked against the code: 2026-10-15 (branch `main`, commit `3ad337c`).
> This file explains how Hometown Comeback was built, why it was built that way, and how someone
> (a person or another AI tool) can take it over. It links to the project's other docs instead
> of repeating them. If this file and the code disagree, the code wins; fix this file.

## 1. What it is and who uses it
Hometown Comeback is a planned cozy browser game. The player moves back to a worn-down hometown (Millbrook) and
rebuilds one Main Street, one shop at a time. Version 1 scope: one Main Street, five shops, 30 levels. It is
for women 35 and older, with a warm tone, gentle humor and 1970s to 1990s nostalgia. It is meant to be a solo-mode
game in the partygamesarcade.com family, free in the browser.

Status: idea only, on hold. Doug said not to build it right now. Nothing has been built: there is no code,
no art, no mockups, no mechanics and no dialogue trees. What exists is a design draft (shops, characters, tone).
It is not live.

## 2. Where it runs

| Piece | Where | Notes |
|---|---|---|
| Live site / app | not live | Plan says to host it as a page on partygamesarcade.com |
| Hosting | not set up yet | |
| Domain and DNS | not set up yet | partygamesarcade.com is the planned home; how it is hosted is unknown, check the party-game repo |
| Build and publish path | none | No code exists |
| Database | none | v1 plan: files stay on the device, no accounts. Save system (device storage or account) is an open question |
| Server code / workers | none | |
| Scheduled jobs (timers) | none | |
| Email / SMS | none | |
| Analytics and ads | not set up yet | Rule: GA4 on the public site once a property exists |
| Repo | `dugwdn/hometown-comeback`, default branch `main` | No other long-lived branches known |

## 3. How it was built
- Stack: not chosen. The repo holds only Markdown documents.
- Folder map: `CLAUDE.md` (rules, state, plan, open questions), `README.md` (short summary), and
  `docs/shops-and-characters.md` (the design draft, about 290 lines).
- Data model: none. The five shops, their townspeople and the story arcs are described in the design draft only.
- Migrations or data updates: none.
- Tests: none.

What the design draft covers: a player backstory, the five shops in unlock order (Ruby's Diner, The Melody Record
Shop, Rosewood Theater, The Leaf & Petal Garden Shop, Vintage Threads Consignment), each with a townsperson,
a 3-part story arc, a nostalgia detail, 3 decorating styles and a seasonal event, plus a relationship web that
ends in a shared Friday Night gathering.

## 4. Why it was built this way
- Design first, no code: Doug's rule for new games is to get 2-3 style mockups and his approval of a look before any art is built.
- Free first and files on the device: the rules in `CLAUDE.md` say to ask Doug before spending money and to need no accounts in v1.
- Audio after launch, CC0 sources only (Kenney, Freesound CC0, OpenGameArt), so licensing stays simple.
- Story and tone live in `docs/shops-and-characters.md`, which `CLAUDE.md` calls the source of truth.
- No decision records, PRD or roadmap exist. The plan is in `CLAUDE.md`.

## 5. Accounts and services
None used so far. If it is built: GitHub (`dugwdn/hometown-comeback`, Doug's account), partygamesarcade.com hosting
(account unknown, check the party-game repo), and GA4 once a property exists. No secrets or environment variables exist.

## 6. Run it on Doug's Windows laptop
There is nothing to run yet. To read the design draft:
1. Open VS Code, File, Open Folder, `C:\Users\doug\Documents\hometown-comeback`. If the folder is missing, clone it first:
```
cd C:\Users\doug\Documents
git clone https://github.com/dugwdn/hometown-comeback
```
2. In the left panel open `docs/shops-and-characters.md`. Press Ctrl+Shift+V to see it formatted.

## 7. Publish, roll back, check health
Not applicable: there is nothing to publish. When a game exists, decide the hosting path with Doug (the plan says a page on partygamesarcade.com) and write it here.

## 8. Recurring jobs and what breaks if they stop
None.

## 9. Known issues and quirks
- On hold by Doug's choice. Do not start building without his go-ahead.
- Names are unchecked: "Hometown Comeback" and the town name "Millbrook" still need a name check.
- The 30 levels are not yet split across the 5 shops (about 6 per shop is the guess in the plan), and what a level is has not been decided.

## 10. Open work
See the "Plan" and "Open questions" sections of `CLAUDE.md`. First step when it restarts: 2-3 warm small-town mockups for Main Street and Ruby's Diner, and Doug picks one.

## 11. Other docs in this repo

| File | What it is |
|---|---|
| `CLAUDE.md` | Rules, current state, plan, open questions |
| `README.md` | Short summary |
| `docs/shops-and-characters.md` | Design draft: shops, characters, story arcs, connections |

There is no PRD, roadmap, TRD, decision records, runbook, test plan or changelog.

## 12. Take over with another bot
```
You are taking over Hometown Comeback (repo dugwdn/hometown-comeback). It is an idea on hold: do not build code or art unless Doug says so. Before changing anything:
1. Read HANDOFF.md, then CLAUDE.md, then docs/shops-and-characters.md.
2. There are no tests yet. If you add code, add tests and run them.
Rules:
- Tone: cozy, warm, gentle humor. The player is a catalyst, not a savior. Era-authentic 70s to 90s details.
- Plays free in the browser on all devices. Say "device", not "phone". Check 390px wide.
- Plays on mute, captions on by default. A full screen button on the game.
- Equal rows (menus, button rows, card grids). No underlined links. No sideways-swipe menus.
- New games get 2-3 style mockups first. Doug approves a look before art is built.
- Free first. Ask Doug before spending money. Audio comes after launch, CC0 sources only.
- Never commit passwords, keys or tokens.
- Work on a new branch and open a pull request; never push straight to main.
- Update HANDOFF.md in the same pull request if you change hosting, the data model, the deploy
  path or a key decision.
Task: <describe the task here>
```

## 13. Take over by hand
1. Doug adds the person on GitHub: repo, Settings, Collaborators, Add people.
2. No service accounts are needed today.
3. Start with the design draft and the "Plan" in `CLAUDE.md`. Running and publishing do not apply until a game exists.
