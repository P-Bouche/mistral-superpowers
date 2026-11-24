# mistral-superpowers — portage Vibe Code

Framework de skills et méthodologie de développement de obra (brainstorming, plans, TDD, revues) porté pour Vibe Code.

Portage des skills de [superpowers](https://github.com/obra/superpowers) (archive de la branche `main`, 24 novembre 2026) vers le format Agent Skills utilisé par Vibe Code. 15 skills.

## Skills portées

- `brainstorming` : "You MUST use this before any creative work - creating features, building components, adding functionality,...
- `diagnosing-mistral-superpowers` : Use when a mistral-superpowers session went wrong and your human partner wants to know why — repeated work, ignored...
- `dispatching-parallel-agents` : Use when facing 2+ independent tasks that can be worked on without shared state or sequential dependencies
- `executing-plans` : Use when executing an implementation plan in the current session as the implementer yourself — your human p...
- `finishing-a-development-branch` : Use when implementation is complete, all tests pass, and you need to decide how to integrate the work
- `receiving-code-review` : Use when receiving code review feedback, before implementing suggestions, especially if feedback seems uncl...
- `requesting-code-review` : Use when completing tasks, implementing major features, or before merging to verify work meets requirements
- `subagent-driven-development` : Use when executing implementation plans with independent tasks in the current session
- `systematic-debugging` : Use when encountering any bug, test failure, or unexpected behavior, before proposing fixes
- `test-driven-development` : Use when implementing any feature or bugfix, before writing implementation code
- `using-git-worktrees` : Use when starting feature work that needs isolation from current workspace or before executing implementati...
- `using-mistral-superpowers` : Use when starting any conversation - establishes how to find and use skills, requiring skill invocation bef...
- `verification-before-completion` : Use when about to claim work is complete, fixed, or passing, before committing or creating PRs - requires r...
- `writing-plans` : Use when you have a spec or requirements for a multi-step task, before touching code
- `writing-skills` : Use when creating new skills, editing existing skills, or verifying skills work before deployment

## Installation

**Option A — comme plugin (expérimental)** : copier ce dossier entier dans `~/.vibe/plugins/mistral-superpowers/`.

**Option B — comme skills individuelles** : copier chaque sous-dossier de `skills/` (sauf `_shared`, qui est un dossier de support) dans `~/.vibe/skills/` ou `~/.agents/skills/` (niveau utilisateur), ou `./.vibe/skills/` / `./.agents/skills/` (niveau projet). Dans une session Vibe Code, `/reload` les prend en compte ; `/skills` les liste.

**Option C — depuis Claude Code** : si les skills sont déjà installées côté Claude Code, `/vibe:import` dans Vibe Code reprend instructions, skills, subagents, hooks et serveurs MCP.

Détail des adaptations : voir `PORT-NOTES.md`.

## Licence

MIT (fichier LICENSE repris du dépôt d'origine)
