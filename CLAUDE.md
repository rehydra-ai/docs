# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Documentation site for [Rehydra](https://github.com/rehydra-ai/rehydra-sdk), an on-device PII anonymization module for high-privacy AI workflows. The docs are built with [Mintlify](https://mintlify.com/).

## Development

```bash
# Install Mintlify CLI (requires Node.js 19+)
npm i -g mintlify

# Start local dev server at http://localhost:3000
mintlify dev
```

Deployment is automatic via the Mintlify GitHub app when changes are pushed to `main`.

## Site Configuration

- `docs.json` — Mintlify configuration: theme, colors, navigation structure, logos, navbar, footer
- Navigation is organized into two tabs: **Documentation** and **API Reference**

## Content Structure

All content pages are `.mdx` files using Mintlify components (`<Card>`, `<CardGroup>`, `<Steps>`, `<CodeGroup>`, `<Tip>`, etc.). Each page has YAML frontmatter with `title` and `description`.

- Root pages: `index.mdx`, `quickstart.mdx`, `installation.mdx`
- `concepts/` — Core concepts (PII types, anonymization pipeline, encryption)
- `guides/` — How-to guides (NER, semantic enrichment, sessions, streaming, LLM proxy, browser usage, custom recognizers)
- `api-reference/` — API docs (createAnonymizer, anonymize, rehydrate, storage, sessions, streaming, proxy, crypto, model management)

## Adding/Reordering Pages

New pages must be added to the `navigation` section in `docs.json` to appear in the sidebar. The page path in `docs.json` omits the `.mdx` extension.

## Assets

- `logo/` — SVG logos for light and dark themes (referenced in `docs.json`)
- `images/` — Image assets
- `favicon.ico` — Site favicon
