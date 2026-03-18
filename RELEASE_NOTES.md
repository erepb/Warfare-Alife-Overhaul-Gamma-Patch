## What's Changed

### Features
- Recall logic from all smart terrains, preventing resource loss during night recall
- Do not recall squads to hostile bases; do not block recall from smarts under attack
- Patrol squads convert to random patrols after losing their base
- PDA tooltip shows squad distribution by type (normal/patrol/random patrol) and target squad names
- Add patrol squad type to tooltip
- Invasion: under_attack true only for actual invasions, with configurable depart time control
- Color-coded target icons — cyan for planned attacks, red for under attack
- Replace red circle with tinted faction icon when under attack
- Highlight player's faction smarts under attack
- More balanced balanced preset

### Bug Fixes
- Fix squad-squad targeting
- Fix patrol spawning
- Fix mutant movement from non-empty smarts
- Fix find_targets_for_overflow calls
- Fix smart info display in tooltip
- Fix squads getting stuck after completing player's order
- Remove Darkscape from main ISG base list
- Update patrol idle timer when night activity roll fails
- Exclude mutants from under_attack invasion defense logic
- Fix keep last base protects only base
- Do not retarget attack squads to victims
