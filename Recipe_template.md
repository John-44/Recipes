# Recipe template

This file sets out how every recipe in this repository is written. Follow it whenever you create or edit a recipe, whether you are a person or an LLM.

**To write a new recipe:**

1. Copy [the template](#the-template) into a new file in the `recipes/` folder, named as described in [File names](#file-names).
2. Fill in every `{placeholder}`, following the [rules](#rules) for each section.
3. Delete any optional section you don't need.
4. If the recipe uses another recipe as an ingredient, add it to that recipe's **Used in** section.
5. Check your work against the [checklist](#checklist).

## Sections at a glance

Keep the sections in this order.

| Section | Required? | What goes in it |
| --- | --- | --- |
| Title | Yes | The name of the dish |
| Description | Yes | What the dish is, in 100 words or fewer |
| Summary box | Yes | Prep time, cook time, total time and servings |
| Equipment | Optional | Kit beyond the basics |
| Ingredients | Yes | Everything you need, in the order you use it |
| Directions | Yes | Step 1, Step 2 and so on |
| Notes and substitutions | Optional | Tips, swaps and shortcuts |
| Storage and make-ahead | Optional | Fridge, freezer, make-ahead and reheating |
| Used in | Component recipes only | Recipes that use this one as an ingredient |
| Origin | Yes | The country and region the dish comes from |
| Tags | Yes | Category tags |
| Sources | Yes | Where the recipe's ideas came from |

## The template

```markdown
# {Recipe Title}

{What the dish is, what it tastes like, and how to serve it. 100 words max.}

| Prep time | Cook time | Total time | Servings |
| --- | --- | --- | --- |
| {15 min} | {30 min} | {45 min} | {4} |

## Equipment

- {Item} ({alternative, if there is one})

## Ingredients

### {Group name, only if the recipe has more than one part}

- {amount} {unit} {ingredient}, {preparation}
- {amount} {unit} [{Linked Recipe Title}]({Linked_recipe_title}.md)
- {ingredient}, to taste

## Directions

**Step 1: {Short title}.** {What to do, how hot, how long, and how to tell when it's done.}

**Step 2: {Short title}.** {...}

## Notes and substitutions

- **{Topic}:** {Tip, swap or shortcut.}

## Storage and make-ahead

- **Fridge:** {How long it keeps and how to store it.}
- **Freezer:** {How long it keeps and how to thaw it.}
- **Make ahead:** {What you can do in advance.}
- **Reheat:** {How to reheat it.}

## Used in

- [{Recipe Title}]({Recipe_title}.md)

## Origin

- **Country:** {Country}
- **Region:** {Region}

## Tags

- {Tag}
- {Tag}

## Sources

- {Website}: [{Page title}]({URL}). {What this recipe took from it.}
```

## Rules

### Writing style

- Write for a home cook who has never made the dish.
- Use plain English and short sentences.
- Write directions as instructions: "Fry the onion", not "The onion should be fried".
- Be specific. Give amounts, times, heat levels and sizes. Avoid vague words like "some", "a little" or "a while".
- Explain an unusual technique in a few words the first time it appears, e.g. "Crack the coconut cream (fry it until the oil separates)."
- Use British English spelling and UK ingredient names: coriander, spring onions, aubergine, courgette, red pepper, prawns, chillies, plain flour, double cream.
- Write numbers as digits: "2 minutes", not "two minutes".
- Call each ingredient by the same name everywhere in the recipe.
- No life stories, adverts or hype ("the best ever").
- Write in your own words. Don't copy text from sources.

### File names

- All recipes go in the `recipes/` folder. No subfolders.
- The file name is the recipe title in Sentence_case: a capital first letter, everything else lower case, underscores instead of spaces, and `.md` on the end.
- Leave out apostrophes, accents and other punctuation.

| Title | File name |
| --- | --- |
| Thai Yellow Curry Paste | `Thai_yellow_curry_paste.md` |
| Pad Thai | `Pad_thai.md` |
| Mum's Lasagne | `Mums_lasagne.md` |
| Crème Brûlée | `Creme_brulee.md` |

### Linking to other recipes

- Link with the file name only. All recipes are in the same folder, so no path is needed: `[Thai Yellow Curry Paste](Thai_yellow_curry_paste.md)`.
- The link text is the other recipe's title, exactly as written.
- Link a recipe where it appears in the ingredient list. In the directions, just use its name.
- You can also link from **Notes and substitutions**, e.g. "For a chicken version, see [Thai Yellow Chicken Curry](Thai_yellow_chicken_curry.md)."
- Only link to recipes that exist. If the one you need doesn't exist yet, write it first using this template, or list the ingredient without a link.
- If a store-bought version works, add `(or store-bought)` to the ingredient line and give details in **Notes and substitutions**.
- If you rename or delete a recipe, update every link to it.

### Title

- Use Title Case and the name a UK cook would recognise.
- Include the main ingredient when the dish comes in several versions: "Thai Yellow Prawn Curry", not "Yellow Curry".
- Use an English name, unless the dish is best known in the UK by its original name (e.g. "Pad Thai"). Mention the original name in the description instead.
- Don't use brackets in the title.

### Description

- 100 words max. Two to four sentences is usually enough.
- Say what the dish is, what it tastes like, what makes this version good, and how to serve it.
- Give the dish's original name if it has one, e.g. "Known in Thailand as *gaeng garee*."
- Warn the cook about anything they need to know before they start, such as overnight marinating or another recipe that must be made first.

### Summary box

- Write times as `10 min`, `1 hr` or `1 hr 30 min`.
- **Prep time:** hands-on time preparing ingredients, such as chopping, measuring and pounding.
- **Cook time:** time on the hob or in the oven. Write `None` if there's no cooking.
- **Total time:** prep time + cook time + any waiting time (soaking, marinating, resting, cooling).
- Times are for this recipe only. Don't include the time it takes to make linked recipes.
- **Servings:** the number of people it feeds, e.g. `4`.
- For a component recipe (a paste, sauce, stock, dressing or spice mix), rename the **Servings** column to **Makes** and give the amount, e.g. `About 125 ml (enough for 1 curry for 4)`.

### Equipment

- List only kit a basic kitchen might not have, e.g. a mortar and pestle, spice grinder, stick blender, wok, or a 20 cm square cake tin.
- Give an alternative in brackets if there's a good one: `- Mortar and pestle (or a stick blender)`.
- Don't list the basics: knives, chopping boards, pans, bowls, spoons, scales, measuring spoons and jugs.

### Ingredients

Write each ingredient on its own line, in the order you use it:

`- {amount} {unit} {ingredient}, {preparation} ({short note})`

```markdown
- 500 g raw king prawns, peeled and deveined
- 2 lemongrass stalks, white part only, finely sliced
- 1 can (400 ml) coconut milk
- 4 tbsp [Thai Yellow Curry Paste](Thai_yellow_curry_paste.md) (or store-bought)
- 1 tbsp palm sugar, grated (or soft brown sugar)
- 1 cup Thai basil leaves, loosely packed
- Salt, to taste
```

- Name each ingredient as you'd find it in a UK shop: "raw king prawns", "unsalted butter", "plain flour".
- Put the preparation after a comma: "finely chopped", "peeled and deveined".
- Use brackets for short notes only, such as `(optional)` or a quick swap. Put longer advice in **Notes and substitutions**.
- If the recipe has distinct parts, group the ingredients under `###` subheadings, such as `### For the marinade` and `### To serve`.

#### Measurements

| Measure | Use it for | Example |
| --- | --- | --- |
| g, kg | Solid ingredients: meat, fish, vegetables, flour, sugar, rice, noodles | `500 g raw king prawns` |
| ml, L | Liquids over 4 tbsp | `250 ml chicken stock` |
| tsp, tbsp | Small amounts of anything, up to 4 tbsp: spices, salt, sauces, oil, pastes | `2 tbsp fish sauce` |
| cups | Light, bulky ingredients that are awkward to weigh and don't need to be exact: loose herbs and leaves, cooked rice | `1 cup Thai basil leaves, loosely packed` |
| cans | Ingredients sold in cans, when you use the whole can | `1 can (400 g) chopped tomatoes` |
| Count | Things you naturally count | `4 garlic cloves`, `2 eggs` |
| To taste | Seasoning you adjust at the end | `Salt, to taste` |

- 1 tsp = 5 ml, 1 tbsp = 15 ml and 1 cup = 250 ml. Spoon measures are level unless the recipe says "heaped".
- A standard can is 400 g (or 400 ml for liquids such as coconut milk). Always give the size in brackets: `1 can (400 g) chickpeas, drained and rinsed`, `2 cans (400 g each) chopped tomatoes`.
- If you only use part of a can, give the amount in g or ml instead: `200 ml coconut milk`.
- Never use cups for flour, sugar, butter or anything else that needs to be accurate. Weigh it.
- Round to amounts that are easy to measure: `250 g`, not `247 g`. Switch to kg and L from 1,000: `1.2 kg`, `1.5 L`.
- Use ½, ⅓, ⅔, ¼ and ¾ with spoons, cups, cans and counts (`1½ tsp`). Don't use fractions with g or ml.
- Give a size for counted items when it matters (`1 large onion`), and a rough weight when it matters a lot (`1 large potato (about 300 g)`).
- Put a space between the number and the unit: `500 g`, `2 cm`.

### Directions

Write each step as its own paragraph, starting with a bold step number and a short title:

```markdown
**Step 1: Fry the paste.** Heat the coconut cream in a wok over medium-high heat until it bubbles and the oil starts to separate, about 3 minutes. Add the curry paste and fry, stirring, until fragrant, about 2 minutes.

**Step 2: Simmer the potatoes.** Add the potatoes, coconut milk and stock. Simmer over medium heat until the potatoes are just tender, about 15 minutes.
```

- Each step covers one stage of cooking, in 1–3 short sentences.
- Start the step title with a verb and keep it to 2–5 words: "Fry the paste."
- Say how hot (low, medium, medium-high or high heat), how long, and how to tell when it's done: "until golden, about 5 minutes".
- Write "minutes" and "hours" in full here. Only the summary box uses `min` and `hr`.
- Give oven temperatures in °C with the fan temperature in brackets: `200°C (180°C fan)`.
- Use the same ingredient names as the ingredient list. Only repeat an amount when you split an ingredient between steps: "Add half the coconut milk (200 ml)."
- If the ingredients are grouped, use matching `###` subheadings here too. Keep counting steps across groups. Don't restart at Step 1.
- Finish with how to serve.

### Notes and substitutions

- Write one bullet per note, starting with a bold topic: `- **Store-bought paste:** Brands vary in heat and saltiness, so start with less and add more to taste.`
- Keep each note to 1–2 sentences.
- Useful things to include:
  - Swaps for hard-to-find ingredients, and where to buy them (e.g. "Asian supermarkets").
  - A store-bought swap for a linked recipe, with the amount to use.
  - How to make the dish milder or hotter.
  - Other main ingredients that work, with a link if this repository has that recipe.
  - Dishes or ingredients with similar names that are easy to confuse.

### Storage and make-ahead

- Use these labels, and leave out any that don't apply: **Fridge**, **Freezer**, **Make ahead**, **Reheat**.
- Follow UK food safety guidance from the [Food Standards Agency](https://www.gov.uk/government/publications/how-to-chill-freeze-and-defrost-food-safely/how-to-chill-freeze-and-defrost-food-safely) and the NHS:
  - Cool leftovers and put them in the fridge within 1–2 hours. Eat them within 2 days.
  - Eat cooked rice within 24 hours, and reheat it only once.
  - Thaw frozen food in the fridge, and eat it within 24 hours of thawing.
  - Reheat food until it's steaming hot all the way through.
- For the freezer, up to 3 months is a safe default.
- If you're not sure how long something keeps, give the shorter time.

### Used in

- Only component recipes have this section: pastes, sauces, stocks, dressings, spice mixes and anything else used as an ingredient in other recipes.
- List every recipe in this repository that uses this one as an ingredient, in alphabetical order.
- When a new recipe uses a component, add the new recipe to the component's **Used in** list at the same time.

### Origin

- Give where the dish itself comes from, not where this version was created.
- **Country:** the country's current English name, e.g. `Thailand`.
- **Region:** the region, state, province or city it comes from, e.g. `Southern Thailand`, `Sichuan` or `Naples`.
- If the dish comes from the whole country rather than one region, write `Nationwide`.
- If experts disagree, give the most widely accepted answer, add `(disputed)`, and explain in one sentence in **Notes and substitutions**.
- Don't guess. If you can't find a reliable answer, write `Unknown`.

### Tags

- Each tag is a single category: `Pastes`, not `Pastes and sauces`. If two categories apply, use two tags.
- Choose from the tag list below, spelled exactly as shown.
- Every recipe needs at least one **Type** tag. Add **Course**, **Main ingredient** and **Diet** tags where they apply.
- List tags one per line, in alphabetical order.
- Don't tag the country or cuisine. That's what **Origin** is for.
- Only use a **Diet** tag if the whole recipe qualifies, including linked recipes. For example, fish sauce and shrimp paste aren't vegetarian, and ordinary soy sauce contains wheat, so it isn't gluten-free.
- If no tag fits, add a new one to the list below (following the same rules), then use it.

| Group | Tags |
| --- | --- |
| Course | Breakfasts, Desserts, Drinks, Mains, Sides, Snacks, Starters |
| Type | Breads, Cakes, Curries, Dressings, Marinades, Pastes, Pickles, Salads, Sauces, Soups, Spice mixes, Stews, Stir-fries, Stocks |
| Main ingredient | Beef, Chicken, Eggs, Fish, Lamb, Noodles, Pasta, Pork, Pulses, Rice, Seafood, Tofu, Vegetables |
| Diet | Dairy-free, Gluten-free, Vegan, Vegetarian |

### Sources

- List every website, video or book that shaped the recipe, one per line:
  `- {Website}: [{Page title}]({URL}). {What this recipe took from it.}`
- For example: `- Serious Eats: [Prik Gaeng Garee (Thai Yellow Curry Paste)](https://www.seriouseats.com/prik-gaeng-garee-yellow-curry-paste-5190967). Toasting the spices before grinding.`
- Use the page's real title and full URL. Only include links you have opened and checked. Never make one up.
- For a book, give the title, author and page number instead of a link.
- If the recipe is entirely your own, write `- None. This is an original recipe.`

## Checklist

- [ ] The file is in `recipes/` and named as described in [File names](#file-names).
- [ ] The description is 100 words or fewer.
- [ ] Total time = prep time + cook time + any waiting time.
- [ ] Every ingredient is used in the directions, and every ingredient in the directions is in the list.
- [ ] Measurements follow the [measurement rules](#measurements), and every can has its size.
- [ ] Every link points to a recipe that exists, and the link text matches its title.
- [ ] Each linked component recipe lists this recipe under **Used in**.
- [ ] **Origin** has a country and a region.
- [ ] Tags come from the [tag list](#tags), or you've added new ones to it.
- [ ] Every source URL is real and you have checked it.
- [ ] Optional sections with nothing in them have been deleted.
- [ ] No `{placeholders}` are left.
