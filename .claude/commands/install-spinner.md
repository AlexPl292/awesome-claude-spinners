Ask the user which spinner pack they want to install. List all available `.json` files from the `spinners/` directory in this repository (without the `.json` extension).

Present the packs to the user in a table with three columns: Pack name, a short description, and a couple of example verbs. Use the table from `README.md` as reference for descriptions and examples.

Let the user pick one.

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

After successful installation, print:

```
Spinner pack "<pack-name>" installed successfully!
No need to restart Claude Code — the new spinners are active immediately.
```

## Removing spinners

If the user asks to remove or reset spinners, read `~/.claude/settings.json` and delete the `spinnerVerbs` field entirely. Do not modify any other fields. After removal, print:

```
Spinner pack removed. Default spinners are back.
No need to restart Claude Code — the change takes effect immediately.
```
