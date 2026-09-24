# Sauces: Freezer Sauce Library

Make-ahead sauces that freeze and reheat well, for chicken, fish, steak and pasta. Each one should batch
cleanly, freeze in meal-sized portions, and reheat to something close to fresh.

This section works alongside the sous vide / freezer meal-prep routine: proteins vacuum-sealed raw, rice
portioned, sauce frozen in ice cube trays.

Tracked in Jira: [HOUSE-39](https://ryan-kolean.atlassian.net/browse/HOUSE-39)

## Index

A sauce lives in one folder but is listed under every category it pairs with. Status: ✅ finished ·
🧪 testing · 📝 stub.

### Compound butters: [`compound-butters/`](compound-butters/)

| Butter | Pairs with | Status |
| --- | --- | --- |
| [Cacio e pepe](compound-butters/cacio-e-pepe-butter.md) | pasta | 📝 |
| [Lemon](compound-butters/lemon-butter.md) | pasta, fish | 📝 |
| [Garlic-anchovy-chile](compound-butters/garlic-anchovy-chile-butter.md) | pasta, steak | 📝 |
| [Sage brown butter](compound-butters/sage-brown-butter.md) | pasta | 📝 |
| [Nduja / Calabrian chile](compound-butters/nduja-calabrian-chile-butter.md) | pasta | 📝 |
| [Herb-garlic](compound-butters/herb-garlic-butter.md) | pasta, steak, fish | 📝 |
| [Miso](compound-butters/miso-butter.md) | pasta, fish | 📝 |
| [Peppercorn](compound-butters/peppercorn-butter.md) | steak | 📝 |
| [Blue cheese](compound-butters/blue-cheese-butter.md) | steak | 📝 |
| [Lemon-dill](compound-butters/lemon-dill-butter.md) | fish | 📝 |

### Pasta: [`pasta/`](pasta/)

| Sauce | Status |
| --- | --- |
| [Cacio e pepe sauce](pasta/cacio-e-pepe-sauce.md) | ✅ (freezer untested) |
| [Basic tomato](pasta/basic-tomato.md) | 📝 |
| [Bolognese / ragù](pasta/bolognese.md) | 📝 |
| [Arrabbiata / marinara variants](pasta/arrabbiata-marinara.md) | 📝 |
| [Pesto](pasta/pesto.md) | 📝 |
| [Lemon pasta sauce](pasta/lemon-pasta-sauce.md) | 📝 |
| Compound butters: cacio e pepe, lemon, garlic-anchovy-chile, sage brown, nduja, herb-garlic, miso | see above |

### Chicken: [`chicken/`](chicken/)

| Sauce | Status |
| --- | --- |
| [Lemon-herb pan sauce](chicken/lemon-herb-pan-sauce.md) | 📝 |
| [Soy-ginger glaze](chicken/soy-ginger-glaze.md) | 📝 |
| [Mustard-cream base](chicken/mustard-cream-base.md) | 📝 |
| [Chimichurri](steak/chimichurri.md) (in `steak/`) | 📝 |

### Fish / salmon: [`fish/`](fish/)

| Sauce | Status |
| --- | --- |
| [Lemon-dill sauce](fish/lemon-dill-sauce.md) | 📝 |
| [Miso glaze](fish/miso-glaze.md) | 📝 |
| [Soy-ginger glaze](chicken/soy-ginger-glaze.md) (in `chicken/`) | 📝 |
| Compound butters: lemon, lemon-dill, miso, herb-garlic | see above |

### Steak: [`steak/`](steak/)

| Sauce | Status |
| --- | --- |
| [Red wine reduction](steak/red-wine-reduction.md) | 📝 |
| [Peppercorn sauce](steak/peppercorn-sauce.md) | 📝 |
| [Chimichurri](steak/chimichurri.md) | 📝 |
| Compound butters: herb-garlic, peppercorn, blue cheese, garlic-anchovy-chile | see above |

---

## Workstream 1: Compound butters

**Freeze the fat, not the emulsion.** A compound butter has no emulsion to break, so it comes through
freezing and thawing with no change in texture. The sauce is emulsified fresh in the pan with hot pasta and
starchy water. That makes sauces that used to be fresh-only possible to prep ahead, and it will probably be
the backbone of this library.

### Build rules

- **Zest, not juice.** Acid and free water make a thawed butter weep. Zest carries the flavor; add fresh
  juice in the pan if it needs brightening.
- **How starchy the water is matters more than how much there is.** Cook pasta in less water than usual so
  the water is genuinely starchy. Or keep reduced pasta water on hand, or use a small cornstarch slurry so
  results are repeatable.
- **Emulsify off the heat.** Melt the butter into the hot pasta with starchy water, away from direct heat,
  tossing hard.
- **Brown or toast aromatics first**, then chill them before working them into the butter.

### Portioning

- Silicone molds or ice cube trays give exact, repeatable portions. Use them instead of slicing a log.
- Starting ratio to test: **~28 g butter per serving of pasta**
- Label with name, date and finishing instructions.

### Using one butter for several proteins

Test whether one butter can cover more than one category (for example herb-garlic on pasta, steak and fish)
to keep the library small.

## Workstream 2: Conventional freezer sauces

Tomato-based sauces, reductions and glazes, frozen finished or nearly finished.

### Freezer standard

- Ice cube trays (1–2 oz) for pan sauces; 1-cup containers or bags frozen flat for pasta sauces
- Label with sauce name, date and reheat notes
- Target shelf life: 3–4 months
- Freeze flat where possible so it thaws fast

### Known limits

- **Sauces heavy on dairy separate.** Freeze the base; add cream, butter or cheese at reheat.
- **Sauces thickened with a roux can go grainy.** Thicken by reduction, or with a cornstarch slurry after
  thawing.
- **Fresh herbs turn dark and lose their punch.** Add them at service.

## Test protocol

For each sauce or butter:

1. Make a full batch. Taste and rate it fresh (the baseline).
2. Portion and freeze.
3. Thaw one portion at **1 week** and one at **4 weeks**.
4. Reheat or finish it and rate it against the fresh baseline: texture, separation, flavor strength.
5. Record what to change (thicken more up front, hold back the dairy, change the starch ratio, and so on).
6. Mark pass or fail, write the final recipe, and set `status: finished` and `freezer: pass|fail`.

## Done when

- [ ] At least one sauce passes for each of: chicken, fish, steak, pasta
- [ ] Cacio e pepe compound butter passes, or its failure is written up with reasons
- [ ] Ratio of butter to pasta water established and repeatable
- [ ] Each keeper has a written recipe with batch size, freeze format and finishing instructions
