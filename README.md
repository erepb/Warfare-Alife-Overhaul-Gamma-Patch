How to contribute:
1) Gamma patch should always have mod_offline_combat_simulator_warfare.ltx but `[stationary_squads]` should be always dltx'ed to `![stationary_squads]`

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


