## What's Changed

### Improvements
- Levels added by other addons derive a mutant cap from the lairs they actually have, so they no longer depend on being listed by name; level packs that register their own cap keep it
- Underground levels added by level packs use the lab mutant cap and rare-mutant chance when the pack declares them a lab
- Levels whose smart terrains opt out of the simulation, no longer count towards a level's mutant cap
- A missing global position is reported once per level and object instead of on every call, which kept a single misconfigured level from filling the log

### Bug Fixes
- Fix a crash on levels added by other addons: the mutant spawner multiplied by a per-level cap that only covered the 34 vanilla levels
- Fix mutants being placed in areas whose smart terrains opt out of the simulation
- Fix new-game mutant seeding rolling for every lair regardless of the level's mutant cap
- Fix new-game seeding using the northern rare-mutant chance for Jupiter Underground and X8 instead of the lab chance
- Fix smart terrain positions being resolved before level packs have registered their level offsets
