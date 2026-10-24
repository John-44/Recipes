# Recipe template

This file sets out how every recipe in this repository is written. Follow it whenever you create or edit a recipe, whether you are a person or an LLM. Use it together with the [Terminology glossary](Terminology_glossary.md), which pins the exact words the recipes use.

**To write a new recipe:**

1. Read the [Terminology glossary](Terminology_glossary.md).
2. Copy [the template](#the-template) into a new file in the `recipes/` folder, named as described in [File names](#file-names).
3. Fill in every `{placeholder}`, following the [rules](#rules) for each section. Wherever the glossary has a term for something, use it exactly. In **Credits**, put yourself as the **Original author**.
4. Delete any optional section you don't need.
5. If the recipe uses another recipe as an ingredient, add it to that recipe's **Used in** section. That counts as editing that recipe, so add yourself to its **Editors** too, unless you're already credited there.
6. Add every new term the recipe uses to the glossary, as described in [Terminology](#terminology).
7. Check your work against the [checklist](#checklist).

**To edit a recipe:**

1. Read the [Terminology glossary](Terminology_glossary.md).
2. Make your changes, following the [rules](#rules) for each section you change.
3. Add yourself to the recipe's **Editors**, unless you're already credited there, as described in [Credits](#credits).
4. Add every new term your changes use to the glossary, as described in [Terminology](#terminology).
5. Check your work against the [checklist](#checklist).

For complete examples, see [Thai Yellow Curry Paste](recipes/Thai_yellow_curry_paste.md) and [Thai Yellow Prawn Curry](recipes/Thai_yellow_prawn_curry.md).

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
| Tags | Yes | Category tags, grouped into Course, Type, Main ingredient and Diet |
| Credits | Yes | Who added the recipe, and who has edited it since |
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

- **Fridge:** {How long it keeps}, or up to {time} if vacuum packed. {How to store it.}
- **Freezer:** {How long it keeps}, or up to {time} if vacuum packed. {How to thaw it.}
- **Make ahead:** {What you can do in advance.}
- **Reheat:** {How to reheat it.}

## Used in

- [{Recipe Title}]({Recipe_title}.md)

## Origin

- **Country:** {Country}
- **Region:** {Region}

## Tags

- **Course:** {Tag}
- **Type:** {Tag}
- **Main ingredient:** {Tag}
- **Diet:** {Tag}, {Tag}

## Credits

- **Original author:** [{GitHub username}](https://github.com/{GitHub username})
- **Editors:** [{GitHub username}](https://github.com/{GitHub username}), [{GitHub username}](https://github.com/{GitHub username})

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
- Call each thing by the same name every time, in this recipe and every other. Use the terms in the [Terminology glossary](Terminology_glossary.md), as described in [Terminology](#terminology).
- No life stories, adverts or hype ("the best ever").
- Write in your own words. Don't copy text from sources.

### Terminology

The [Terminology glossary](Terminology_glossary.md) pins the exact words the recipes in this repository use: ingredients, equipment, dish names, preparation and cooking terms, headings and labels, shops, origins, tags and sources. It stops recipes drifting apart, with one asking for "coriander leaves" and the next for "fresh coriander".

**Before you start:** read the glossary, whether you're writing a new recipe or editing one.

**While you write:**

- When the recipe needs something the glossary lists, use its term exactly: the same words, spelling, hyphens, word order and capitals.
- Never call something by a name in its **Don't use** column.
- In the ingredient list, write each ingredient's full term. After that, you can shorten it as far as its **Short name**: "raw king prawns" in the list can be "the prawns" in the directions.
- If two ingredients in the same recipe would end up with the same short name, keep more of each term, such as "dried chillies" and "red chilli".
- Only reuse a term when it means exactly the same thing. If you need something different, such as ground ginger rather than ginger, give it a new term. Don't stretch an existing term to fit, or reword it to suit one recipe.

**When you've finished:**

- Add every term the recipe uses that isn't in the glossary yet, including swaps that appear only in **Notes and substitutions**. Put each one in the right section and family, at the place the glossary's [ordering rules](Terminology_glossary.md#how-the-tables-are-ordered) give it, not at the end of the table. Fill in its columns as described in [How the entries work](Terminology_glossary.md#how-the-entries-work).
- Before you add a term, check it isn't another name for something the glossary already has. If it is, change the recipe to use the existing term.

**When you change a term or delete a recipe:**

- Don't change an existing term just because you prefer another word. If a term really does need to change, change it in the glossary and in every recipe that uses it, at the same time.
- If no recipe uses a term any more, remove it from the glossary. Tags are the exception: the tag list keeps every tag.

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
- If a store-bought version works, add `(or store-bought, see Notes)` to the ingredient line and give details in **Notes and substitutions**.
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
- **Total time:** start to finish, including any waiting time (soaking, marinating, resting, cooling). Don't count time twice when things overlap, such as chopping while something soaks.
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
- 2 lemongrass stalks, top half and tough outer layers removed, finely sliced
- 1 can (400 ml) coconut milk
- 4 tbsp [Thai Yellow Curry Paste](Thai_yellow_curry_paste.md) (or store-bought, see Notes)
- 1 tbsp palm sugar, grated (or soft light brown sugar)
- 1 cup Thai basil leaves, loosely packed
- Salt, to taste
```

- If the [glossary](Terminology_glossary.md#ingredients) lists the ingredient, use its term exactly. If it doesn't, name the ingredient as you'd find it in a UK shop, such as "raw king prawns", "unsalted butter" or "plain flour", and add it to the glossary.
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
- Say how hot (low, medium-low, medium, medium-high or high heat), how long, and how to tell when it's done: "until golden, about 5 minutes".
- Write "minutes" and "hours" in full here. Only the summary box uses `min` and `hr`.
- Give oven temperatures in °C with the fan temperature in brackets: `200°C (180°C fan)`.
- Use the same ingredient names as the ingredient list, or shorten them as far as their [glossary](Terminology_glossary.md#ingredients) short names: "the prawns" for raw king prawns. Only repeat an amount when you split an ingredient between steps: "Add half the coconut milk (200 ml)."
- If the recipe has separate parts, such as a marinade and a sauce, you can use matching `###` subheadings here too. A `### To serve` ingredient group doesn't need one. Keep counting steps across subheadings. Don't restart at Step 1.
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
- For food that isn't vacuum packed, up to 3 months in the freezer is a safe default.
- If you're not sure how long something keeps, give the shorter time.

#### Vacuum packing

UK food safety guidance doesn't give longer storage times for food you vacuum pack at home, so this repository takes its vacuum-packed times from a maker of professional vacuum packing machines instead. Always assume the cook uses a chamber vacuum packer, which can vacuum pack wet food, such as curries, in a bag.

- If the recipe can be vacuum packed, end the first sentence of its **Fridge** and **Freezer** entries with how long it keeps that way: `Up to 2 days in an airtight container, or up to 10 days if vacuum packed.`
- Take the time from the vacuum-packed column of the entry closest to the finished recipe in [Turbovac's shelf life table](https://turbovac.nl/shelf-life-table/), and list the table in **Sources**. For example, a curry is closest to "Cooked food". A curry paste, made mostly of fresh herbs and vegetables, fits both the herb and the vegetable entries.
- Use Turbovac's vacuum-packed time as it is, even when it's much longer than the time without vacuum packing, such as 18 months against 3 months in the freezer. The 3-month default above is only for food that isn't vacuum packed.
- If more than one entry fits, or an entry gives a range, use the shortest time. If no entry is close, or Turbovac's tips say the food can't be vacuum packed, leave vacuum packing out.
- If vacuum packing doesn't make it keep any longer, say so in one go: `Up to 1 week, either vacuum packed or in an airtight container.`
- Leave vacuum packing out of an entry that says the food doesn't keep there, such as a **Freezer** entry that says `Not recommended`.
- For a paste, say to freeze it until solid before vacuum packing it. The vacuum then stops it getting freezer burn: `To vacuum pack it, freeze it flat until solid, then vacuum pack it.`
- Vacuum pack food as soon as it has chilled. Turbovac says food keeps longer the fresher and cleaner it is when it's packed.
- A vacuum-packed time replaces the 2-day limit for leftovers, but the rest of the food safety guidance above still applies: get food into the fridge within 1–2 hours, eat cooked rice within 24 hours, thaw food in the fridge and eat it within 24 hours, and reheat it until it's steaming hot all the way through.

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
- Choose from the [tag list](Terminology_glossary.md#tags) in the Terminology glossary, spelled exactly as shown.
- Every recipe needs at least one **Type** tag. Add **Course**, **Main ingredient** and **Diet** tags where they apply.
- Give each group its own line: the group's name in bold, then its tags, separated by commas, as in `- **Diet:** Dairy-free, Gluten-free`.
- Keep the groups in the tag list's order: **Course**, **Type**, **Main ingredient**, then **Diet**. Leave out any group with no tags.
- On each line, put the tags in the order the tag list gives them.
- Don't tag the country or cuisine. That's what **Origin** is for.
- Only use a **Diet** tag if the whole recipe qualifies, including linked recipes. For example, fish sauce and shrimp paste aren't vegetarian, and ordinary soy sauce contains wheat, so it isn't gluten-free.
- If no tag fits, add a new one to the glossary's tag list (following the same rules), then use it.

### Credits

- Name each person by their GitHub username, exactly as GitHub shows it, linked to their GitHub profile: `[John-44](https://github.com/John-44)`. Don't use the name on their profile, which can be blank and can change.
- **Original author:** the person who first committed the recipe to this repository.
- **Editors:** everyone else who has had a pull request that changes the recipe merged into `main`. List each person once, in the order of their first merged change, separated by commas.
- Never list the original author as an editor, even if they edit the recipe later.
- If no one else has edited the recipe, leave out the **Editors** line.
- Any merged change to the recipe's file counts, however small, including a change made to every recipe at once, such as renaming a term. Credit the person who opened the pull request, not the co-authors of its commits.
- Update the credits in the same pull request as your change:
  - When you add a recipe, add yourself as **Original author**.
  - When you change a recipe you're not credited on yet, add yourself to the end of its **Editors** line. If your pull request isn't merged, your credit goes with it.
  - If you're an LLM, credit the person whose GitHub account will open the pull request. If you're not sure who that is, ask.

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
- [ ] Total time is start to finish, including any waiting time.
- [ ] Every ingredient is used in the directions, and every ingredient in the directions is in the list.
- [ ] Measurements follow the [measurement rules](#measurements), and every can has its size.
- [ ] Every link points to a recipe that exists, and the link text matches its title.
- [ ] The **Fridge** and **Freezer** entries follow the [vacuum packing rules](#vacuum-packing).
- [ ] Each linked component recipe lists this recipe under **Used in**.
- [ ] **Origin** has a country and a region.
- [ ] Tags come from the [tag list](Terminology_glossary.md#tags), or you've added new ones to it, and each group is on its own line, in the tag list's order.
- [ ] You're credited in **Credits** on every recipe you've added or changed.
- [ ] Everything the [Terminology glossary](Terminology_glossary.md) lists is called by its exact term or short name, and nothing is called by a name from a **Don't use** column.
- [ ] Every new term the recipe uses has been added to the glossary.
- [ ] Every source URL is real and you have checked it.
- [ ] Optional sections with nothing in them have been deleted.
- [ ] No `{placeholders}` are left.
