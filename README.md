How to contribute:
1) The Warfare patch declares `[stationary_squads]` (in `mod_offline_combat_simulator_warfare_stationary.ltx`), a section that does **not** exist in vanilla `offline_combat_simulator.ltx`. It must always be dltx'ed as `@[stationary_squads]` — the DLTX "safe override" operator. `@` creates the section when no other addon declares it, and merges (unions) with declarations from other addons (e.g. Dux's Innumerable Characters Kit) instead of raising a duplicate-section fatal. Do **not** use `![stationary_squads]`: `!` only overrides a section that already exists and will not create it, so Warfare's stationary squads would silently fail to register whenever no other addon declares the section. (Use `![section]` only for sections that exist in vanilla, e.g. `![offline_health]`.)

2) Commit messages must follow the **Conventional Commits** format, as they are used to automatically bump the version and generate the changelog on release:

   ```
   <type>: <description>
   ```

   | Type | When to use | Version bump |
   |---|---|---|
   | `feat` | New feature or addition | minor (x.**y**.0) |
   | `fix` | Bug fix | patch (x.y.**z**) |
   | `perf` | Performance improvement | patch |
   | `refactor` | Code restructure, no behavior change | patch |
   | `chore` | Maintenance, CI, deps — not shown in changelog | none |

   Add `!` after the type for **breaking changes** — bumps the major version (e.g. `feat!: rework spawn logic`).

   Examples:
   ```
   feat: add dynamic faction reinforcements
   fix: prevent infinite spawn loop after GAMMA update
   perf: reduce squad evaluation overhead
   feat!: replace static squad tables with dynamic config
   ```

Changelog:
Fixes after 1.5 version from discord:

- avoid the infinite spawns brought on by the newest gamma update by @notkc


