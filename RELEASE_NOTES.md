## What's Changed

### Features
- Save and delete warfare presets from the options screen: name a preset, store the current warfare settings in it, and pick it back up from the preset dropdown
- Hawkie's Warfare Mechanic Fix is bundled for non-GAMMA installs, so toolkits handed to a Warfare faction mechanic reach the workbench

### Improvements
- Removed the per-faction "Participate in Warfare" setting - every faction always takes part in warfare
- Factions in the balanced preset now target levels they are not directly linked to
- Emergency resurrection spawns at least four squads instead of at most four

### Bug Fixes
- Fix option descriptions only showing for one faction group - every faction now gets hover tooltips
- Add the option descriptions that were missing entirely, in English and Russian
- Fix "Ignore empty targets" doing nothing: factions with it enabled no longer target unowned locations
- Fix the emission zone purge percentage defaulting to 50 instead of 5
- Fix crash from a nil global position in the offline combat distance multiplier
