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
| [Cowboy](spinners/cowboy.json) | Wild West & frontier | "Lassoing the solution", "Riding into the sunset" |
| [Zombie](spinners/zombie.json) | Zombie apocalypse survival | "Reanimating dead code", "Double-tapping the bug" |
| [Therapist](spinners/therapist.json) | Therapy speak & self-care | "Holding space for the code", "Unpacking that" |
| [Ninja](spinners/ninja.json) | Ninja & stealth | "Moving through the shadows", "Striking silently" |
| [Ocean](spinners/ocean.json) | Ocean & underwater | "Diving into the deep end", "Surfing the data waves" |
| [Startup](spinners/startup.json) | Startup culture | "Disrupting the industry", "Iterating on the MVP" |
| [Time Traveler](spinners/time-traveler.json) | Time travel & paradoxes | "Firing up the flux capacitor", "Rewriting the timeline" |
| [Superhero](spinners/superhero.json) | Superhero themed | "Suiting up", "Saving the day" |
| [Gardening](spinners/gardening.json) | Gardening & growing | "Planting the seed", "Pulling the weeds" |
| [90s Kid](spinners/90s-kid.json) | 90s nostalgia | "Dialing up the internet", "Blowing into the cartridge" |
| [Vibecoder](spinners/vibecoder.json) | Vibe coding culture | "Letting the AI cook", "Shipping on good vibes" |
| [Vim](spinners/vim.json) | Vim editor enthusiasts | "Exiting vim (attempting)", "Yanking the line" |
| [SF Entrepreneur](spinners/sf-entrepreneur.json) | San Francisco tech scene | "Grabbing a Blue Bottle coffee", "Cold-emailing a16z" |
| [Michael Scott](spinners/michael-scott.json) | The Office's Michael Scott | "Declaring bankruptcy on the old code", "Somehow managing" |
| [Walter White](spinners/walter-white.json) | Breaking Bad's Heisenberg | "Being the one who codes", "Going full Heisenberg" |
| [The Dude](spinners/the-dude.json) | Big Lebowski's The Dude | "Abiding", "Sipping a White Russian" |
| [Borat](spinners/borat.json) | Borat Sagdiyev | "Very nice! Great success-ing", "High five-ing the compiler" |
| [Darth Vader](spinners/darth-vader.json) | Star Wars' Sith Lord | "Finding your lack of tests disturbing", "Force-pushing to the remote" |
| [Yoda](spinners/yoda.json) | Star Wars' Jedi Master | "Reading the code, I am", "Trying not, doing" |
| [Blue Collar Dev](spinners/blue-collar-dev.json) | Trades & construction humor | "Hammering out code", "Duct-taping that together" |
| [Honest No Filter](spinners/honest-no-filter.json) | Brutally honest dev thoughts | "Making it worse first", "Hoping this compiles" |
| [Sarcastic AI](spinners/sarcastic-ai.json) | Self-aware AI humor | "Hallucinating responsibly", "Confidently guessing" |

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
