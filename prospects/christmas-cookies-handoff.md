# Handoff: Christmas Cookies (the 24)

Session notes so the work can continue in a local Claude Code session. Delete this file once the work is
picked up.

## Where things are

- **Repo:** `ryankolean/food-lab`
- **Branch:** `ccr-c1133d23-8m7hw8`, pushed. No PR opened.
- **Main file:** [`prospects/christmas-cookies.md`](christmas-cookies.md). It has:
  - the 24-day calendar (recipe, link, evidence, grade A/B/C)
  - a "What each one is" table: main elements, flavor, and what makes each exceptional
  - category coverage, what was left out and why, a bench of 9 alternates, open questions, and links
    to the bake-off sources
- **Also changed:** `README.md` and `prospects/README.md` each got one row linking the new file.

To pick up locally:

```bash
git fetch origin ccr-c1133d23-8m7hw8
git checkout ccr-c1133d23-8m7hw8
```

## What was asked, in order

1. Research the internet for the highest-rated Christmas cookies and cut the list to 24, advent-calendar
   style, keeping only cookies that are truly worth it. **Done** (first draft).
2. The user isn't sure they like all of them and wanted the main elements, a short description of the
   taste, and what makes each exceptional. **Done**: the "What each one is" table.
3. The user wants to include the Petit Demi Christmas cookies:
   https://www.petitdemi.com/categories/christmas-cookies. **Started, not finished.** See below.

## Petit Demi: what's known so far

The category page was downloaded once and lists these 9 recipe links:

| Recipe | URL |
| --- | --- |
| Caramel Cornflake Cups | https://www.petitdemi.com/recipes/caramel-cornflake-cups |
| Chai White Chocolate Toffee Cookies | https://www.petitdemi.com/recipes/chai-white-chocolate-toffee-cookies |
| Chocolate Chunk Shortbread Cookies | https://www.petitdemi.com/recipes/chocolate-chunk-shortbread-cookies |
| Cinnamon Spiced Homemade Caramels | https://www.petitdemi.com/recipes/cinnamon-spiced-homemade-caramels |
| Classic Butter Cookies | https://www.petitdemi.com/recipes/classic-butter-cookies |
| Gingerbread Men | https://www.petitdemi.com/recipes/gingerbread-men |
| Millionaire's Chocolate Chip Cookies | https://www.petitdemi.com/recipes/millionaires-chocolate-chip-cookies |
| Raspberry Thumbprint Cookies | https://www.petitdemi.com/recipes/raspberry-thumbprint-cookies |
| Vanilla Choco Pinwheel Cookies | https://www.petitdemi.com/recipes/vanilla-choco-pinwheel-cookies |

A web search also surfaced these as Christmas-related on the site, but they were not among the links on
the category page (check for pagination or a second page):

- Cheesecake Stuffed Red Velvet Cookies: https://www.petitdemi.com/recipes/cheesecake-stuffed-red-velvet-cookies
- Almond Frangipane Cookies (Dutch *gevulde koeken*, speculoos-spiced version at Sinterklaas and
  Christmas): https://www.petitdemi.com/recipes/almond-frangipane-cookies
- White Chocolate, Pistachio and Raspberry Cookies: https://www.petitdemi.com/recipes/white-chocolate-pistachio-and-raspberry-cookies

From search snippets only (individual pages not read yet):

- Raspberry thumbprints: soft, buttery, jam center; dough freezes baked or unbaked; makes about 20.
- Chocolate chunk shortbread: slice-and-bake logs, chill 2 hours, 180 °C for 12–15 minutes.
- Chai white chocolate toffee: browned butter, warm spices, white chocolate, toffee bits, toasted
  pecans; chill scooped dough 1 hour to overnight.
- Gingerbread men: rolled to 6 mm, 175 °C for 9–11 minutes, royal icing.
- Caramel cornflake cups: no-bake, mini muffin tin, about 20.

### Next steps for Petit Demi

1. Read each recipe page (and check the category page for a second page).
2. Ask the user whether "include" means all of them or a pick, and whether they replace existing slots
   or push the list past 24 (the 24 cap was the user's rule).
3. Points to raise when deciding, not yet discussed with the user:
   - **Not cookies:** cinnamon caramels (candy) and caramel cornflake cups (no-bake cups).
   - **Direct overlaps with current picks:** chocolate chunk shortbread vs day 4 (Alison Roman);
     raspberry thumbprints vs day 15 (Sugar Spun Run); gingerbread men vs day 12 (Tartine) and the other
     ginger cookies (days 9, 14).
   - **Previously excluded types:** pinwheels (reviews call them bland) and red velvet (bland, low
     ratings). The Petit Demi versions may be different; worth saying so.
   - **Chocolate chip:** the house already has finished chocolate chip recipes, so Millionaire's
     chocolate chip was outside the original brief.
4. Add Petit Demi picks to `christmas-cookies.md` in the same format: calendar row, "What each one is"
   row, and move displaced picks to the bench.

## Other open work

- **Verify the research.** In the cloud session no recipe or bake-off page could be opened, so every
  rating, count and bake-off placing in `christmas-cookies.md` came from search-result text. Locally
  there's no network block, so confirm each against the live page. The "Open questions" section in that
  file lists the specific conflicts (Pancake Princess sugar cookie placings, crinkle winner, two
  links from memory: gochujang caramel cookies and Allrecipes biscotti).
- **The user's doubts about the picks.** The user hasn't said which ones they dislike yet. Overlaps
  that may help them cut: three ginger cookies (9, 12, 14), three shortbread-style (4, 6, 13) plus
  snowballs (11), three jam cookies (7, 15, 22), two frosted sugar cookies (13, 24). Weakest-evidence
  picks: buckeyes (8), peppermint bark (19), Linzer (22).
- **Not done:** no recipes stubbed into `baking-and-desserts/`. Each pick should become a stub from
  `templates/recipe.md` once the list is settled and the source page has been read (grams, Jira ticket,
  "from the source" vs "added later" notes, per the repo conventions in `README.md`).
- **No Jira ticket** was created or assigned for this list. Other sections use HOUSE-xx tickets.

## Repo conventions to keep

- One recipe per Markdown file, kebab-case, in its section folder, from `templates/recipe.md`.
- Front matter: status (`stub` / `testing` / `finished`), yield, source, jira.
- Weigh in grams.
- Keep what came from the source separate from anything added or guessed.

## Suggested opening prompt for the local session

> Read `prospects/christmas-cookies-handoff.md` and `prospects/christmas-cookies.md`. Read every Petit
> Demi recipe listed in the handoff, then show me each one in the same format as the "What each one is"
> table, with how it compares to the current pick it overlaps. Then help me decide which go into the 24.
