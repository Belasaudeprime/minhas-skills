# minhas-skills

Skills do Claude Code, empacotadas como marketplace de plugins para funcionar em qualquer PC.

| Plugin | Skills | Origem |
|---|---|---|
| design-skills | frontend-design | anthropics/skills |
| | web-design-guidelines, react-best-practices, composition-patterns, react-native-skills | vercel-labs/agent-skills |
| | ui-ux-pro-max | nextlevelbuilder/ui-ux-pro-max-skill |
| | bencium-controlled-ux-designer | bencium/bencium-claude-code-design-skill |
| accesslint | accessibility-audit, -scan, -inspect, -fix, -diff | accesslint/claude-marketplace |

## Instalar num PC novo

Adicione em `~/.claude/settings.json` :

```json
{
  "extraKnownMarketplaces": {
    "minhas-skills": { "source": { "source": "github", "repo": "Belasaudeprime/minhas-skills" }, "autoUpdate": true }
  },
  "enabledPlugins": {
    "design-skills@minhas-skills": true,
    "accesslint@minhas-skills": true
  }
}
```

Requisitos opcionais: Python (busca da UI/UX Pro Max), Node.js e Chrome (AccessLint).
