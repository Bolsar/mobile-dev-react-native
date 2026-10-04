---
name: mobile-dev-react-native
description: React Native Stack Pack for the mobile-dev agent (TypeScript + Expo). Use for any React Native app work - writing, reviewing, testing, verifying or releasing React Native code - together with the mobile-dev skill.
---

# React Native Stack Pack

Requires the **mobile-dev** plugin. If the mobile-dev agent isn't loaded yet, load the `mobile-dev` skill first; this pack only adds the React Native specifics.

Files, relative to the pack root: `../../` from this SKILL.md (`${CLAUDE_PLUGIN_ROOT}` in Claude Code, `.mobile-agent/stacks/react-native/` in a copied install):

| File | Holds | Read it when |
|---|---|---|
| `defaults.md` | Greenfield picks, project layout, wiring | Starting a project or feature with no existing convention |
| `idioms.md` | Concurrency, lifecycle, UI idioms, classic bugs | Writing or reviewing React Native code |
| `tooling.md` | Toolchain, lint, test, profiling, release, done check | Setting up, verifying or shipping |
| `verify` | Lint + tests + Maestro flow + screenshot and logs into `.mobile-agent-proof/` | Proving a change works |

Run verify from the app project's root: `<pack root>/verify [--flow .maestro/<flow>.yaml]`.

Rules:
- **Existing project wins.** A pick in `defaults.md` is for greenfield only. If the project already uses another library for the same job, keep it and flag only real problems.
- **Versions move.** Library names here are stable picks, not pinned versions. Check the current docs and the project's lockfile before adding or upgrading anything, and check the min OS before using a newer API.
- Stack-agnostic rules live in mobile-dev `references/core/`. This pack only says how they look in React Native.
