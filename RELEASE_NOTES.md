## What's Changed

### Features
- Limit invasions to 1 per 5 bases
- Protect main bases completely from attacks (option-gated)
- Allow capture for all factions
- Show invasion info for neutral factions
- Show raw and distance-adjusted squad power in tooltip
- Show when patrol spawn is capped
- Consolidate max spawn timers into single multiplier option
- Add option to convert squads to zombies during emission
- Pull patrols back during night recall
- Update balanced preset

### Bug Fixes
- Fix stack overflow
- Fix combat disengage distance consistency
- Fix squad power reset after combat disengage
- Fix distance power multiplier
- Fix formatted invasion timer
- Fix forces advancing tooltip
- Hide target for non-player squads
- Allow overflow from bases at all times except night
- Keep last squad on loner/ecolog main bases
- Reset invasion departure when base loses squads
- Properly call on_death after combat
- Retask random patrols on arrival

### Internal
- Refactor main base registry and story mode travel restrictions
- Refactor Miracle Machine and Brain Scorcher restrictions
- Optimize squad_count and sim_squad_scripted.show
- Move logging under debug flag, reduce log spam
