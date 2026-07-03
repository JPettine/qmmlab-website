# AGENTS.md

## Project context

This is an Astro-based research group website. The site should be clean, academic, modern, and easy to maintain.

## Working style

- Make small, targeted edits.
- Do not refactor unrelated files.
- Do not rewrite large sections unless explicitly asked.
- Prefer simple, readable code over clever abstractions.
- Before editing, identify the specific files that need changes.
- After editing, summarize exactly what changed and which files were modified.
- If a request is ambiguous, make the smallest reasonable interpretation rather than changing broad parts of the site.

## Speed rules

- Do not run `npm install` unless dependencies are missing.
- Do not run `npm run dev` unless specifically asked.
- Do not run a full build for small text, CSS, or image path changes unless needed.
- Prefer inspecting known files over searching the whole repository.

## Astro rules

- Use Astro conventions.
- Static images should usually go in `public/images/`.
- Reference images from `public/images/` as `/images/filename.ext`.
- Do not put large binary assets in `src/` unless there is a reason to use Astro image optimization.
- Keep component structure simple.

## Design rules

- Use consistent page structure: present major content in similarly styled boxes/panels, with the small red eyebrow labels placed above the boxes rather than inside them unless there is a specific design reason not to.
- Preserve the existing visual direction unless explicitly asked to redesign.
- For the QMM / Quantum Meta Matter branding, do not alter approved logo assets unless explicitly asked.
- Avoid generic startup-style design.
- Prefer refined academic/nano/quantum visual language.
- Use responsive layouts that look good on desktop and mobile.

## Asset / binary file rules

- Do not modify, restore, replace, or commit binary assets unless explicitly requested.
- If an image appears distorted, first fix the page markup or CSS to preserve the existing asset's intrinsic aspect ratio rather than changing the image file.
- Before committing, check `git diff --stat` and ensure unintended binary file changes are reverted.

## Git / safety rules

- Never delete files unless explicitly asked.
- Never overwrite existing assets without asking.
- Do not add new production dependencies without asking first.
- Do not commit secrets, API keys, tokens, or credentials.
- Do not change deployment settings unless explicitly asked.

## Response format

At the end of each task, report:

1. Files changed
2. What changed
3. Any commands run
4. Anything the user needs to do manually
