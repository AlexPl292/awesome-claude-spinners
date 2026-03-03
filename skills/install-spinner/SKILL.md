---
name: install-spinner
description:
  Install themed spinner verb packs for Claude Code. Fetches spinner packs
  directly from the awesome-claude-spinners repository and installs them into
  the user's settings. Use when the user wants to customize their Claude Code
  spinner, install spinner verbs, or change spinner themes.
license: MIT
metadata:
  author: alexpl292
  version: '1.0.0'
---

# Install Spinner

Install themed spinner verb packs for Claude Code from the
[awesome-claude-spinners](https://github.com/alexpl292/awesome-claude-spinners) repository.

## Steps

1. Fetch the list of available spinner packs from GitHub:

```
https://api.github.com/repos/alexpl292/awesome-claude-spinners/contents/spinners
```

Parse the JSON response to get the list of `.json` files. Extract the pack names by removing the `.json` extension.

2. Present the list of available packs to the user and ask them to pick one.

3. Once the user picks a pack, fetch its contents from:

```
https://raw.githubusercontent.com/alexpl292/awesome-claude-spinners/main/spinners/<pack-name>.json
```

4. Read the user's `~/.claude/settings.json` file.

5. Copy the `spinnerVerbs` field from the fetched spinner JSON into `~/.claude/settings.json`. If the `spinnerVerbs` field already exists in `settings.json`, replace its value. If it doesn't exist, create it.

IMPORTANT: Do not modify any other fields in `settings.json`. Only change `spinnerVerbs`.
