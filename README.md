# Awesome Claude Spinners [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of spinner verb packs for [Claude Code](https://docs.anthropic.com/en/docs/claude-code)

Claude Code displays spinner verbs like "Thinking...", "Analyzing..." while processing your requests. You can customize these with themed verb packs to make your coding sessions more fun.

## What are Spinners?

When Claude Code is working on a task, it shows a spinner with rotating verb phrases:

```
⠋ Analyzing your codebase...
⠙ Refactoring the module...
⠹ Deploying to prod on Friday...
```

You can replace the default verbs with any themed set you like!

## Installation

1. Pick a spinner pack from the list below
2. Copy the JSON contents
3. Merge it into your `~/.claude/settings.json`:

```json
{
  "spinnerVerbs": {
    "mode": "replace",
    "verbs": [
      "Your custom verb one",
      "Your custom verb two"
    ]
  }
}
```

Or use `"mode": "append"` to add verbs to the defaults instead of replacing them.

## Spinner Packs

| Pack | Description | Sample Verbs |
|------|-------------|--------------|
| [Developer](spinners/developer.json) | Programming & dev culture | "Deploying to prod on Friday", "Rewriting in Rust" |
| [Corporate](spinners/corporate.json) | Corporate buzzwords & jargon | "Synergizing", "Circling back" |
| [Motivational](spinners/motivational.json) | Hype & motivational phrases | "Absolutely crushing it", "Leveling up" |
| [Meme](spinners/meme.json) | Internet memes & viral phrases | "Yeeting the bugs", "Going sicko mode" |
| [Philosophical](spinners/philosophical.json) | Deep thoughts & philosophy | "Pondering existence", "Contemplating the void" |
| [Pirate](spinners/pirate.json) | Pirate speak | "Plundering the codebase", "Sailing the seven repos" |
| [Cat](spinners/cat.json) | Cat-themed | "Knocking things off the table", "Napping on the keyboard" |
| [Space](spinners/space.json) | Space & sci-fi | "Initiating hyperdrive", "Scanning the sector" |
| [Coffee](spinners/coffee.json) | Coffee & food themed | "Brewing a fresh pot", "Letting it simmer" |
| [Retro Gaming](spinners/retro-gaming.json) | Retro gaming references | "Inserting coin", "Loading save file" |
| [Wizard](spinners/wizard.json) | Fantasy & magic themed | "Casting a spell", "Consulting the ancient scrolls" |
| [Detective](spinners/detective.json) | Noir detective style | "Following the trail", "Cracking the case" |
| [Gym Bro](spinners/gym-bro.json) | Gym & fitness culture | "Crushing the set", "Going beast mode" |
| [Shakespeare](spinners/shakespeare.json) | Shakespearean & old English | "Prithee, a moment", "Once more unto the breach" |
| [Chaos](spinners/chaos.json) | Absurdist & chaotic humor | "Flipping the table", "Sacrificing a semicolon" |
| [Wholesome](spinners/wholesome.json) | Wholesome & cozy vibes | "Watering the plants", "Believing in you" |

## Mix & Match

You can combine verbs from multiple packs! Just merge the `verbs` arrays from different packs into a single list in your `settings.json`. For example, mix Developer + Chaos for chaotic dev energy:

```json
{
  "spinnerVerbs": {
    "mode": "replace",
    "verbs": [
      "Deploying to prod on Friday",
      "Rewriting in Rust",
      "Flipping the table",
      "Sacrificing a semicolon"
    ]
  }
}
```

## Contributing

Want to add your own spinner pack? See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

[MIT](LICENSE)
