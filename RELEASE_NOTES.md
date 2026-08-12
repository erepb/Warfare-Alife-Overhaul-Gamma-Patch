## What's Changed

### Features
- Player squad command: take direct control of friendly squads from the PDA map, group them into named detachments, and issue attack, move and follow orders
- Command capacity is derived from the actor's rank, with a configurable cap on commanded squads
- Warfare gets its own PDA tab on engine builds with dynamic tab support, instead of taking over Contacts
- Squad command lives in map context submenus, with a fallback for engine builds without submenu support
- Faction map icons are outlined instead of tinted, so icon addons keep working: yellow for planned targets, orange for imminent invasions, red for bases under attack
- New optional patch: alternative New Levels layout from "It's Warfare Time" by LostToTheSzone, with more faction bases, territories and starting squads on the new maps

### Improvements
- Ecologists and free stalkers now scale their squad count with the number of bases they hold
- Rebalanced faction respawn and patrol timings in the balanced preset
- Removed obsolete max_faction_respawn and max_patrol_time entries from all presets
- Removed the Dux patch and updated the DLTX syntax of the offline combat simulator patch

### Bug Fixes
- Fix loner bases emptying out as squads were sent away
- Fix context menu separators being drawn when no purchase is available
- Fix the warfare PDA tab name
- Fix FOMOD description indents
