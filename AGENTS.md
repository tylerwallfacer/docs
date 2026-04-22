> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Terminology

{/* Add product-specific terms and preferred usage */}
{/* Example: Use "workspace" not "project", "member" not "user" */}

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

{/* Define what should and shouldn't be documented */}
{/* Example: Don't document internal admin features */}

## Keeping docs in sync with the API

The API Reference endpoint pages are auto-generated from the OpenAPI spec and update automatically on every push. No manual work needed there.

The following pages are manually maintained. When making changes that add, rename, or remove API fields or endpoints, update the relevant pages below before closing the PR:

- `concepts/vault-data.mdx` — complete field reference for vault objects. Update when fields change in `/v2/detailed-vaults`, `/v2/portfolio`, `/v2/historical`, or `/v2/nrt`.
- `api-reference/general.mdx`, `detailed-vaults.mdx`, `historical.mdx`, `benchmarks.mdx`, `portfolio.mdx`, `transactions.mdx`, `nrt.mdx` — section overview pages with endpoint tables. Update if endpoint paths or summaries change.
- `api-reference/beta.mdx` and `api-reference/alpha.mdx` — feature descriptions for pre-stable endpoints. Update when beta/alpha features graduate or change scope.

The practical trigger: when you write a changelog entry for a new or changed field, update the relevant page above at the same time.
