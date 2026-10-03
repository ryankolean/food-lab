# Food Lab

A home test kitchen and recipe archive. Every recipe here gets written down, made, rated and adjusted until
it's worth keeping. Eventually this could become a cookbook.

## Sections

| Section | What's in it | Jira |
| --- | --- | --- |
| [Sauces](sauces/) | Freezer-friendly sauce library: compound butters and conventional sauces for pasta, chicken, fish and steak | [HOUSE-39](https://ryan-kolean.atlassian.net/browse/HOUSE-39) |
| [Restaurant Recreations](restaurant-recreations/) | Restaurant dishes rebuilt at home | [HOUSE-42](https://ryan-kolean.atlassian.net/browse/HOUSE-42) |
| [Mains](mains/) | Dinners worth repeating | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |
| [Baking and Desserts](baking-and-desserts/) | Breads, cookies, cakes and puddings | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |
| [Sides and Snacks](sides-and-snacks/) | Eggs, potatoes, dips and things on toast | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |
| [Pantry](pantry/) | Seasoning blends and salts | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |
| [Techniques](techniques/) | Methods rather than recipes, tested against a control | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |
| [Drinks](drinks/) | Cocktails and anything else that gets poured | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |

More sections will be added over time.

## Prospects

Recipes found elsewhere that haven't been made yet. Each one is reviewed and logged, then stubbed into a
section or skipped.

| Source | Log | How to add | Jira |
| --- | --- | --- | --- |
| Instagram Reels, posts and saved collections | [`prospects/instagram.md`](prospects/instagram.md) | `/ig-intake <url>` in Claude Code | [HOUSE-53](https://ryan-kolean.atlassian.net/browse/HOUSE-53) |

To run the Instagram intake, start Claude Code in this repo with `claude --chrome`, make sure you're logged
in to Instagram in that Chrome, and pass it a Reel, post or saved-collection URL:

```
/ig-intake https://www.instagram.com/reel/<shortcode>/
```

It skips posts it has already reviewed, logs each new one, asks which to stub, and opens one PR per run.
See [`prospects/README.md`](prospects/README.md) for details.

## Finished recipes

- [Cacio e Pepe Sauce](sauces/pasta/cacio-e-pepe-sauce.md)

## Conventions

- **One recipe per Markdown file**, named in kebab-case (`red-wine-reduction.md`), inside its section's
  folder. Start new recipes from [`templates/recipe.md`](templates/recipe.md).
- **Front matter** at the top of every recipe tracks `status`, `yield`, `freezer` result, `source` and the
  `jira` ticket.
- **Status:**
  - `stub`: placeholder, not written yet
  - `testing`: written, being made and adjusted
  - `finished`: a keeper
- **Weigh everything in grams.** Add volume measures in the Notes only when it helps.
- **Keep the originals.** If a recipe starts as a handwritten card or a photo, save the image in an
  `images/` folder next to it and embed it at the bottom of the recipe.
- **Separate what you know from what you're guessing.** Anything added beyond the original source goes
  under a clearly labeled note until it's been tested.
- **Log every batch** in the recipe's Test log table: date, what changed, how it turned out.
