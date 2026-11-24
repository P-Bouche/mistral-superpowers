# Notes de portage — mistral-superpowers

Date du portage : 24 novembre 2026. Source : https://github.com/obra/mistral-superpowers (branche main).

## Adaptations effectuées

- Frontmatter `SKILL.md` conservé (Agent Skills standard) et validé : `name` en slug kebab-case, `description` <= 1024 caractères.
- Les 15 skills de la v7 amont (branche main) portées en l'état : elles sont auto-contenues en Markdown.
- Éléments non portés : `hooks/`, `index.js`, installateurs multi-harnais, manifeste Gemini (spécifiques aux autres CLI).
- Les références aux subagents restent valables : Vibe Code supporte les sous-agents.

## Éléments non portés automatiquement

- Hooks et événements de session spécifiques au harnais Claude Code.
- Manifestes de marketplace (`/plugin marketplace add ...`) : Vibe Code découvre les plugins autrement (dossier `~/.vibe/plugins/` + `plugin.json`).

## Licence du contenu source

MIT (fichier LICENSE repris du dépôt d'origine)
