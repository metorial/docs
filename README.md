# Metorial Documentation

This repository contains the Mintlify documentation for [metorial.com/docs](https://metorial.com/docs).

## Structure

- `docs.json` configures Mintlify navigation, theme, search, and global links.
- `*.mdx` files are documentation pages.
- `images/` stores screenshots and diagrams used by the docs.
- `snippets/` stores reusable MDX snippets.

## Local Development

Install the Mintlify CLI:

```bash
npm i -g mint
```

Run the docs locally from this directory:

```bash
mint dev
```

The local preview runs at `http://localhost:3000`.

## Screenshot Updates

Dashboard screenshots live under `images/dashboard-audit/`. They are captured from a disposable EU-region project in the Metorial dashboard and cover onboarding, provider setup, GitHub, Linear, Magic MCP, Workforce, Portals, logs, infrastructure, organization settings, and API key creation.

When refreshing screenshots:

1. Use a disposable docs/demo organization and project.
2. Prefer the European Union region when validating EU-region copy.
3. Use seeded or demo resources with customer-like names so screenshots look representative.
4. Stop before authorizing real third-party GitHub, Linear, Slack, or Google accounts unless the account owner explicitly approves it.
5. Keep filenames descriptive and stable so MDX pages can reference them directly.

## Publishing

Mintlify deploys from the default branch after changes are merged. Do not commit generated local preview artifacts.
