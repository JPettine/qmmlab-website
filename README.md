# QMM Lab Website

This repository contains the Astro scaffold for the QMM Lab website.

## Project structure

```text
/
├── public/
│   └── favicon.svg
├── src/
│   └── pages/
│       └── index.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

Astro routes are created from files in `src/pages/`. Static assets that should be served as-is belong in `public/`.

## Commands

Run all commands from the repository root:

| Command | Action |
| --- | --- |
| `npm install` | Install dependencies |
| `npm run dev` | Start the local development server |
| `npm run build` | Build the production site to `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run astro -- --help` | Show Astro CLI help |

## Recommended next steps

1. Replace the scaffold homepage copy with finalized lab messaging.
2. Add pages for people, research, publications, news, and contact information.
3. Configure deployment once the target host and production URL are known.

## Troubleshooting setup

If `npm create astro@latest` or `npm install` returns `403 Forbidden` from `https://registry.npmjs.org/`, the failure is caused by npm registry access from the current environment rather than by the Astro project files. Check npm registry and proxy settings, then retry dependency installation:

```sh
npm config get registry
npm config get proxy
npm config get https-proxy
npm install
```

The project files in this repository are already scaffolded, so you do not need to run `npm create astro@latest` again unless you intentionally want to regenerate the project.
