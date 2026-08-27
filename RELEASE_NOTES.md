## What's Changed

### Features
- Reworked target scoring: linear distance replaces distance squared, and the priority weights were rebalanced
- Dispatch now contests enemy-held resources and territories instead of only bases
- Patrol destinations are weighted by distance instead of being clipped to the two nearest smarts
- Overflow relocation scores additively, so distance becomes a travel radius rather than a hard cutoff
- Offline squads that merely cross paths now roll for whether they engage, using each faction's patrol hunt chance - deliberate hunts and assaults on a garrison still always engage
- New option to lift the rank-based cap on commanded squads
- The PDA warfare tab sorts factions by power

### Improvements
- Balanced preset updated with playtested faction values

### Bug Fixes
- Fix a crash when the task system scanned a smart terrain whose squad list still referenced a released squad
- Fix squads oscillating between adjacent bases: destination choice now counts squads already in transit, and a base at capacity no longer looks able to receive
- Fix overflow squads with nowhere to go being deleted instead of falling back to their faction HQ
- Fix squads leaving a smart immediately after arriving, and patrols re-picking the smart they are standing on
- Fix overflow relocation targeting smarts too far away
- Fix zombied squads being recalled to bases they do not have: with no main base of their own the recall could only ever fail, and it was retried on every pass over the smart
- Fix night being defined differently in different places - it is now 21:00 to 06:00 everywhere
- Fix min_resurgence_wait_time being unreachable in GAMMA installs which lead to almost immediate resurrection
- Fix resurrection landing on main bases their owner still holds, and move ISG's Agroprom resurrection anchor to a capturable smart
- Fix small factions being unable to launch invasions
- Fix every base of a faction spawning its first defense wave at the same moment
- Fix the base respawn interval never reaching its configured minimum: the curve is anchored at one base instead of zero
- Fix base_count_modifier being applied twice outside update_faction
- Fix the PDA warfare tab reporting base and resource counts inflated by the enemy boosts
- Fix the ImGui timer panels showing a respawn interval the simulation does not use
- Fix a misleading log line about AlifePlus squad release
