> **Customize this file**: Tailor this template to your project by noting specific contribution types you're looking for, adding a Code of Conduct, or adjusting the writing guidelines to match your style.

# Contribute to the documentation

Thank you for your interest in contributing to our documentation! This guide will help you get started.

## How to contribute

### Option 1: Edit directly on GitHub

1. Navigate to the page you want to edit
2. Click the "Edit this file" button (the pencil icon)
3. Make your changes and submit a pull request

### Option 2: Local development

1. Fork and clone this repository
2. Install the Mintlify CLI: `npm i -g mint`
3. Create a branch for your changes
4. Make changes
5. Navigate to the docs directory and run `mint dev`
6. Preview your changes at `http://localhost:3000`
7. Commit your changes and submit a pull request

For more details on local development, see our [development guide](development.mdx).

## Keeping docs in sync with the API

The API Reference endpoint pages are auto-generated from the OpenAPI spec and update automatically on every push. No manual work needed there.

The following pages are manually maintained and should be reviewed whenever the API changelog includes new or changed fields:

- `concepts/vault-data.mdx` — complete field reference for vault objects. Update when fields are added, renamed, or removed from `/v2/detailed-vaults`, `/v2/portfolio`, `/v2/historical`, or `/v2/nrt`.
- `api-reference/general.mdx`, `detailed-vaults.mdx`, `historical.mdx`, `benchmarks.mdx`, `portfolio.mdx`, `transactions.mdx`, `nrt.mdx` — section overview pages with endpoint tables. Update if endpoint paths or summaries change.
- `api-reference/beta.mdx` and `api-reference/alpha.mdx` — feature descriptions for pre-stable endpoints. Update when beta/alpha features graduate or change scope.

The practical trigger: when you write a changelog entry for a new or changed field, that's the signal to update the relevant page above.

## Writing guidelines

- **Use active voice**: "Run the command" not "The command should be run"
- **Address the reader directly**: Use "you" instead of "the user"
- **Keep sentences concise**: Aim for one idea per sentence
- **Lead with the goal**: Start instructions with what the user wants to accomplish
- **Use consistent terminology**: Don't alternate between synonyms for the same concept
- **Include examples**: Show, don't just tell
