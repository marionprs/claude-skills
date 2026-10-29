# claude-skills

Marketplace de plugins Claude Code personnelle, qui versionne mes skills et les synchronise entre mes machines via GitHub.

## Ajouter la marketplace sur une autre machine

```
/plugin marketplace add marionprs/claude-skills
/plugin install mes-skills@claude-skills
```

## Ajouter une nouvelle skill

1. Créer `plugins/mes-skills/skills/<nom>/SKILL.md` (nom en kebab-case, identique au dossier) avec un frontmatter `name:` et `description:`.
2. Bumper la version dans `plugins/mes-skills/.claude-plugin/plugin.json` **et** dans `.claude-plugin/marketplace.json`.
3. Ajouter la skill au tableau ci-dessous.
4. Commit + push.
5. Sur chaque machine : `/plugin marketplace update claude-skills`.

## Skills du plugin `mes-skills`

| Skill | Description |
|---|---|
| `exemple-skill` | Skill d'exemple à remplacer. |
