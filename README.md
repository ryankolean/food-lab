# Food Lab

A home test kitchen and recipe archive. Every recipe here gets written down, made, rated and adjusted until
it's worth keeping. Eventually this could become a cookbook.

## Sections

| Section | What's in it | Jira |
| --- | --- | --- |
| [Sauces](sauces/) | Freezer-friendly sauce library: compound butters and conventional sauces for pasta, chicken, fish and steak | [HOUSE-39](https://ryan-kolean.atlassian.net/browse/HOUSE-39) |
| [Restaurant Recreations](restaurant-recreations/) | Restaurant dishes rebuilt at home | [HOUSE-42](https://ryan-kolean.atlassian.net/browse/HOUSE-42) |

More sections will be added over time.

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
