# Skills — conocimiento reutilizable para Claude

Set de 8 skills basadas en certificaciones Certiprof, escritas para que Claude las use automáticamente cuando el contexto de la conversación lo amerita (no requieren invocación manual).

## Contenido

| Skill | Cubre |
|---|---|
| `design-thinking` | Empatizar-Definir-Idear-Prototipar-Evaluar |
| `lean-six-sigma` | DMAIC — causa raíz, variabilidad, desperdicio |
| `business-intelligence` | ETL, modelado de datos, Power BI / Qlik Sense |
| `prompt-engineering` | Role prompting, few-shot, cadena de pensamiento |
| `ai-literacy` | IA/ML/Deep Learning para audiencia no técnica |
| `data-storytelling` | De insight de datos a narrativa accionable |
| `innovation-management` | Tipos de innovación, árbol de problemas, Lean Startup |
| `project-management-pm2` | Metodología PM² (Comisión Europea) |

Cada carpeta tiene un `SKILL.md` (frontmatter con `name` + `description`, que es lo que activa la skill) y una carpeta `references/` con el resumen del temario oficial.

## Cómo instalarlas

**Claude.ai / Claude Desktop (Cowork):** copiar cada carpeta de skill dentro de tu directorio de skills de usuario (`/mnt/skills/user/` en el entorno, o donde tu organización configure el catálogo de skills).

**Claude Code:** copiar las carpetas dentro de `.claude/skills/` en la raíz del proyecto, o en `~/.claude/skills/` para que estén disponibles en todos tus proyectos.

No requieren instalación de dependencias — son solo Markdown, se activan por coincidencia de contexto con la `description` del frontmatter.

## Licencia / origen

Resúmenes de temarios oficiales de certificaciones Certiprof (Design Thinking, Lean Six Sigma Green Belt, Business Intelligence Analyst, Prompt Engineering Foundation, Generative AI Professional, Data Storytelling, Innovation Management, Project Management Essentials). Uso interno.
