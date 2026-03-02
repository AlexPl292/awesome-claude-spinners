# Contributing to Awesome Claude Spinners

Thanks for wanting to contribute a spinner pack!

## Adding a New Spinner Pack

1. **Fork** the repo and create a new branch
2. Create a new JSON file in the `spinners/` directory
3. Add your pack to the table in `README.md`
4. Submit a pull request

## Spinner Pack Requirements

### File Format

Each spinner pack must be a valid JSON file matching the Claude Code config format:

```json
{
  "spinnerVerbs": {
    "mode": "replace",
    "verbs": [
      "Verb phrase one",
      "Verb phrase two"
    ]
  }
}
```

### Content Rules

- **30-50 verbs** per pack for good variety
- All entries must be **verb phrases** in gerund/present participle form (ending in "-ing" or starting with a verb)
  - Good: "Thinking", "Deploying to prod", "Casting a spell"
  - Bad: "Stonks", "This is fine", "Error 404"
- Keep it **fun and family-friendly** — no slurs, hate speech, or NSFW content
- Each pack should have a clear **theme** — random collections of unrelated verbs aren't useful
- Avoid duplicating verbs that already exist in other packs

### File Naming

- Use lowercase kebab-case: `my-pack-name.json`
- Name should clearly reflect the theme

### README Update

Add your pack to the table in `README.md` with:
- Pack name (linked to the JSON file)
- Short description (under 40 characters)
- Two sample verbs

## Quality Guidelines

- Verbs should be creative and entertaining
- They should make sense as spinner status messages (imagine seeing "Verb..." while waiting)
- Variety is key — avoid too many similar phrases
- Test that your JSON is valid before submitting

## Questions?

Open an issue if you have any questions about contributing!
