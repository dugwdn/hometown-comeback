# Hometown Comeback

Cozy browser game for Doug (Web Design Nerd). Part of the partygamesarcade.com family of games, solo mode. Version 1 scope: one Main Street, 5 shops, 30 levels.

## Game summary
You grew up in Millbrook, left, and now come back. You fix up five shops in this unlock order, each with a townsperson, a 3-part story arc (Rust & Remembering, The Fixing, The Grand Reopening), a nostalgia detail, 3 decorating styles and a seasonal event:
1. Ruby's Diner (Ruby Clearwater, 68)
2. The Melody Record Shop (Marcus Webb, 52)
3. Rosewood Theater (Helen Ashford, 74)
4. The Leaf & Petal Garden Shop (Emma Sutton, 46)
5. Vintage Threads Consignment (Dale Foster, 52)
The five also have a relationship web that ends in a shared Friday Night gathering. Full text: `docs/shops-and-characters.md` (source of truth for story and tone).

## Rules (Doug's standing rules for games)
- **HANDOFF.md (Doug, 2026-10-15, standing):** update HANDOFF.md in the same PR as any change to hosting, domain/DNS, the data model or migrations, the build/deploy path, scheduled jobs, outside services, or a key decision (new ADR).
- Tone: cozy, warm, gentle humor. The player is a catalyst, not a savior. Era-authentic 70s to 90s details.
- Plays free in the browser on all devices. Say "device", not "phone". Check 390px wide.
- Plays on mute, captions on by default. A full screen button on the game.
- Equal rows (menus, button rows, card grids). No underlined links. No sideways-swipe menus.
- Easy / Normal / Hard where it makes sense. A friend-invite text follows the arcade standard if multiplayer is ever added.
- Audio comes after launch (ask Doug "upgrade the audio before promoting?"). Use CC0 sources only (Kenney, Freesound CC0, OpenGameArt).
- Analytics: GA4 on the public site once a property exists.
- New games get 2-3 style mockups first. Doug approves a look before art is built.
- Free first. Ask Doug before spending money.
- Files stay on the device; no accounts needed for v1.

## Current state (2026-10-12)
Design draft done (shops, characters, connections, tone). No mockups, art, dialogue trees, mechanics or code yet.

## Plan
1. Mockups: 2-3 warm small-town looks for Main Street and Ruby's Diner; Doug picks one.
2. Mechanics: restore (clean, fix, decorate) per level; 30 levels = about 6 per shop (draft does not set this yet).
3. Dialogue for first meeting with each character.
4. Playable Ruby's Diner slice, then the other four shops.
5. Music playlist (70s-90s style, licensed or CC0) after launch.
6. Host as a page on partygamesarcade.com.

## Open questions (draft lacks)
- How the 30 levels split across the 5 shops and what a level is (a task? a puzzle? a day?).
- Core gameplay loop and controls (tap-to-clean, match, drag-and-place decoration).
- Art style (mockups needed) and whether portraits are drawn or generated.
- Save system (device storage vs account).
- Name check for "Hometown Comeback" and the town name Millbrook.
