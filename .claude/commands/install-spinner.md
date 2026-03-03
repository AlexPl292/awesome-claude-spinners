Ask the user which spinner pack they want to install. List all available `.json` files from the `spinners/` directory in this repository (without the `.json` extension) and let them pick one.

Once the user has chosen a pack, read the corresponding file from `spinners/<pack-name>.json`. Then read the user's `~/.claude/settings.json` file.

Each spinner file has this format:

```json
{
  "spinnerVerbs": {
    "mode": "replace",
    "verbs": ["Phrase 1", "Phrase 2"]
  }
}
```

Copy the `spinnerVerbs` field from the chosen spinner file into `~/.claude/settings.json`. If the `spinnerVerbs` field already exists in `settings.json`, replace its value. If it doesn't exist, create it.

IMPORTANT: Do not modify any other fields in `settings.json`. Only change `spinnerVerbs`.
