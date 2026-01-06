# Recipe Repository

This is Christian's personal recipe collection, managed with Claude Code.

## About Me

- I live in Berlin, shop mainly at REWE
- I hate mushrooms — never include them, don't suggest them as substitutes
- No food processor or mixer — avoid recipes that require them
- Recipes in English, but use German ingredient names when it helps find things at the store (e.g., "Schmand" not "sour cream")

## Repository Structure

Organize however makes sense. Example:

```
recipes/
├── favorites/       # recipes I love, use them to understand my taste
├── chinese/
├── italian/
├── korean/
├── basics/          # sauces, stocks, techniques
├── other/           # recipes that don't fit a specific cuisine
├── example/         # an example recipe
├── to-try/          # aspirational, haven't made yet
└── archive/         # didn't work out
```

## Units

- Grams for main ingredients (proteins, tofu, pasta, rice, etc.)
- Tablespoons/teaspoons for seasonings, sauces, spices
- "A glug", "a handful" are fine for casual stuff

## How I Use This

- I'll ask to add recipes, update them after cooking, or search for ideas
- When suggesting recipes, look at my favorites to understand what I like
- Don't auto-commit — I'll tell you when to commit
- Commit messages: short and clear, e.g., "Add mapo tofu" or "Update carbonara — more pepper"

## Example Interactions

**Me:** "I made the dan dan noodles yesterday and added extra chili oil, it was great"
**You:** Update the recipe's Notes and Last made date

**Me:** "What should I cook tonight? I have eggs and some leftover rice"
**You:** Suggest options based on ingredients and what I've enjoyed before

**Me:** "Add this recipe I found" + [paste or link]
**You:** Parse it into my format, add to `to-try/`, flag if it contains mushrooms, tag as `vegetarian` if applicable

**Me:** "I want to try something Korean this weekend"
**You:** Check what Korean recipes I have, suggest ones I haven't made recently

## Maintaining CLAUDE_PROJECT_KNOWLEDGE.md

This file is a condensed version of my preferences + top recipes for use in Claude web UI Projects. Keep it in sync:

**Max recipes:** 20

**When to add a recipe:**
- When I add a recipe to `favorites/`
- When I rate a recipe ★★★★☆ or higher

**When at max capacity (20 recipes):**
- Remove the oldest recipe with the same or lower rating that's NOT in `favorites/`
- Priority order: favorites > higher ratings > more recent

**Format:** Keep recipes condensed (ingredients list + short method paragraph)