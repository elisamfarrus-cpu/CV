# AGENTS.md

## Project

Static HTML/CSS/JS CV directory. No build step, no dependencies, no test framework.

## Workflow

- Open `index.html` directly in a browser to preview changes.
- `opencode.json` sets all permissions to `"ask"` — expect confirmation prompts for every tool call.
- No lint, typecheck, or test commands exist. Verify changes visually.

## Conventions

- Photos use `https://picsum.photos/seed/{name}/200/200` for random avatars.
- All CV data is inline in `index.html` inside the `cvs` array (lines ~350-448).
- Design uses dark glamour theme: `#1a1a2e` / `#e2b04a` gold palette, Georgia serif font.

## Git

- Crea commits solo cuando el usuario lo solicita explícitamente.
- Escribe mensajes de commit en presente, concisos y enfocados en el "por qué".
- Verifica con `git status`, `git diff` y `git log` antes de crear un commit.
- No actualizas la configuración de git ni ejecutas comandos destructivos (force push, hard reset) salvo petición explícita.
- No haces amend a commits ya subidos a remoto, salvo que el usuario lo pida y acepte force push.
- Añades solo los archivos relevantes al stage; no haces `git add .` sin revisar.
