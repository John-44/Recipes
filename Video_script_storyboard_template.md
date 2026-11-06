# Recipe video script and storyboard template

Create a complete, tool-independent production brief for a video of any recipe in [The Recipe Repo](README.md). The viewer should be able to follow every technique and understand why the important choices matter. Use the [fully worked Pumpkin Pie example](videos/Pumpkin_pie.md) alongside this template.

This is a template for writing scripts and written storyboards, not a finished video or a requirement to use a particular generation service. Keep the recipe as the source of cooking truth. The storyboard specifies what the AI must show; the dialogue specifies exactly what the cook says.

## Fixed brief

| Item | Requirement |
| --- | --- |
| Destination | YouTube, landscape 16:9. Default delivery: 1920 × 1080, 25 frames per second. These are production choices, not a requirement for a particular model. |
| Length | No longer than 20:00 including titles, transitions and credits; aim for less. Budget from the techniques, not a fixed number of shots. |
| Audience | UK home cooks who have never made the dish. |
| Structure | Introduction and summary, Before you start, Equipment, Ingredients, Directions in numbered recipe order, then the recipe's remaining sections in order. |
| Host | The same man depicted in the current WebP README banner and Terminology glossary illustration, doing all the cooking himself. |
| Voice | Warm, calm British male voice with upper-class Queen's English: clear, cultivated Received Pronunciation, unhurried and welcoming. No parody, pompous vocabulary or imitation of a named person. |
| Visual treatment | Animated oil painting in the repository's Romantic Table style. Real, intelligible cooking movements inside a coherent painted scene. |
| Instruction | Show each distinct preparation and cooking action, its useful result, and its relevant tip. Shorten waiting and repeated motions transparently. |
| Portability | Plain Markdown, explicit source references, stable shot IDs, exact speech and graphics, reusable prompts, and a continuity record. |

## Read and extract before writing

1. Read the recipe in full at a recorded commit, including notes, storage, credits and sources. Read linked component recipes when they affect the preparation shown. Read [Recipe_template.md](Recipe_template.md), [Terminology_glossary.md](Terminology_glossary.md), [Illustration_style_template.md](Illustration_style_template.md) and [Declined_suggestions.md](Declined_suggestions.md).
2. Record the commit, recipe path and relevant image paths. Attach the actual reference images to the downstream tool where possible; a filename or URL alone is not evidence that a tool has seen the image. If references cannot be retrieved, mark that dependency rather than silently inventing a different character.
3. Copy the exact ingredient amounts, ingredient groups, equipment specifications, step titles, temperatures, times, doneness cues and prerequisites into a facts ledger. Preserve British English and the glossary's full terms and permitted short names.
4. Expand every cooking verb into visible actions. Include preparation embedded in ingredient lines, such as peeling or finely chopping, as well as actions in directions. Do not add homemade preparation of a purchased ingredient unless the recipe calls for it. Record where each action will be demonstrated.
5. Map waits and parallel work separately from the editorial running time. Mark conditional actions, optional ingredients, linked components and make-ahead alternatives explicitly. Do not double-count overlapping waits or present alternatives as consecutive mandatory steps.
6. If the source leaves an important cooking decision unresolved or contains conflicting instructions, list the exact issue before production. Do not quietly change the recipe. Ordinary staging choices, such as a consistent bowl colour, can be decided and labelled as production choices.

Recipe fidelity includes the repository's preference for practical technology and reliable measurements. Show a blender, oven, fridge or probe thermometer when required, even in a timeless-looking kitchen. Never substitute a picturesque old technique. Keep processed ingredients where specified; they may be the deliberate best choice.

## Make it engaging through useful progress

Open with the host and a close view of the finished dish within the introduction. State the texture or flavour the viewer is aiming for and the useful technique they will learn. Keep this to about 15–30 seconds, followed by the recipe summary and prerequisites. Mark the opening dish as a preview; reset clearly to uncooked ingredients when the method starts.

Use a repeating teaching pattern: **show the action → show the result → explain the reason while working**. For example, show the crimp being formed, hold on its shape, and explain why the pastry rests. Alternate a welcoming medium shot with clear views of the host's hands and food. Give the viewer small, visible milestones: a smooth mixture, a golden base, a correct thermometer reading, a clean slice.

Let anticipation come from the dish progressing, natural kitchen sounds and the host's reassuring competence. Avoid unrelated stories, claims such as “best ever”, lengthy greetings and repeated requests to subscribe. Do not sacrifice technique coverage for a montage.

## Character, kitchen and visual continuity

### Reference roles

| Reference | Use |
| --- | --- |
| [images/Readme_banner.webp](images/Readme_banner.webp) | Face, curly dark brown hair, light stubble, relaxed expression and the identity of the recipe writer. |
| [images/Terminology_glossary.webp](images/Terminology_glossary.webp) | The same character standing, cream shirt with rolled sleeves, plain cream apron tied at the waist, dark trousers and shoes. Use this cooking outfit consistently. |
| [Illustration_style_template.md](Illustration_style_template.md) and the recipe's WebP | Brushwork, colour, light, food appearance and the recipe-specific serving occasion. |

Use the current WebP README illustration, not the old SVG banner. Establish one character reference sheet from these images before generating clips: front, three-quarter and profile views, full body and hands. This is a downstream production asset to create, not an asset supplied by this Markdown template. Keep the original reference images available for checking any derived sheet.

Lock the host's face, apparent age, hair, stubble, clothing, proportions, voice and handedness across shots. Default staging is right-handed unless changed consistently before production. A hand insert must remain recognisably his, with matching sleeves and skin tone. Do not introduce a second cook or disembodied substitute hands.

Establish a simple kitchen plan: work surface and host positions, window and light direction, oven, fridge, sink and serving surface. Record the positions and appearance of recurring equipment. Keep bowls, ingredient quantities, utensils, pastry shapes and oven settings continuous. A cut must not move an ingredient into a bowl or change its preparation state without showing that action.

### Painted movement, practical clarity

Use layered oil colour, earthy underpainting, visible directional brushwork, translucent shadows, atmospheric blue-grey distance and selective warm highlights. Preserve natural food colours. Food and host belong to the same medium. Keep the working area well lit enough to see fingers, knife placement, mixture texture and doneness.

The illustration guide governs mastheads. For video, adapt its composition deliberately:

- Use 16:9 rather than the masthead's 2:1.
- Give the host prominence when explaining and the hands and food prominence when demonstrating. Keep atmospheric scenery secondary.
- Use overhead views when they clarify handling, alongside three-quarter and close views. Avoid blocking the action with the host's body or a vessel rim.
- Add legible editorial text as a separate layer after image generation. The painted scene itself remains free of invented lettering, labels, logos and watermarks. Accurate tool readouts can also be composited separately.
- Show functional modern cooking equipment. Keep its styling unobtrusive; do not remove controls or change the method to make it look historical.
- Animate actual contact, pressure, movement and material response. No floating tools, instant ingredient changes, malformed fingers or food morphing between states.

For each technique, show a clear starting state, at least one complete readable action cycle and the resulting state. For chopping, show grip, blade motion and cut size before shortening repetitions. For rolling, show pressure and movement before the final shape. For thermometer use, show placement and the reading. Keep these decisive moments at normal speed.

## Speech, sound and graphics

Write exact spoken lines, not “explain the tip”. Use short, natural sentences and direct instructions. The accent changes delivery, not vocabulary: retain the repository's plain English. Explain an unfamiliar term at first use. Address the viewer kindly; give the reason when it changes how they cook.

Aim for about 115–135 spoken words per minute, with pauses around new techniques and numbers. Time a read-through. Allow quiet handling and kitchen sounds; a 20-second shot does not need 20 seconds of speech. Use the host's continuing voice over close-ups of his hands. When his mouth is visible, specify synchronised speech; otherwise use off-camera host speech. Do not add a separate narrator. Never speed up the voice to meet the limit. If the edit exceeds 20:00, shorten repeated footage and introductory or closing material first. Keep every required action and clear demonstration; flag any remaining runtime conflict before generation.

Use natural, action-matched sound: rolling, whisking, chopping, foil, oven door, timer and serving. Default music is absent during instruction; optional quiet original or cleared music can support the opening and end. Never obscure speech or use music as the only time-jump signal.

Default graphic system: warm ivory text on a dark umber translucent panel, with muted amber for time information. Use a simple, legible sans-serif face available to the editor. At 1080p, start with at least 40 px text; enlarge rather than crowd. Keep essential text inside a 5% margin, titles upper left and captions in a reserved lower band. Never cover the working hands, food or thermometer. Use both words and the clock symbol, so colour is not the only cue.

Display ingredient names and exact quantities as they are introduced and added. Page long lists into small groups that can be read, with a pause-to-read cue. Show both conventional and fan oven temperatures. Deliver accurate captions, including meaningful sound labels if needed, and proofread fractions, units, temperatures and timings manually. Do not rely on generated image text or automatic captions for quantities.

## The common time-jump pattern

Use the same pattern in every recipe video. Screen time is the video's running time; process time is the recipe's actual cooking or waiting time. Both belong in the storyboard.

### Waiting

1. Show the host starting the process: setting the timer, placing the dish, closing the door or setting it aside. Say the required duration and any endpoint.
2. Use a 2-second dissolve or card bearing a small amber clock symbol and the exact text pattern **“+{elapsed duration} | {process}”**. The vertical bar separates two text fields; do not put an unescaped bar inside a Markdown table cell. Add a second line with the cumulative process time when needed.
3. Resume on the same object and hold its resulting state clearly for at least 2 seconds before the next action. Retain the time-jump text during this hold, giving at least 4 seconds to read it across the transition and resumed shot. The host names the cue, such as “cold and firm”, before continuing.

The plus sign always means time since the preceding process checkpoint, not time since the beginning of the film. Write durations in full on cards: “+35 minutes | Pastry resting in freezer”, followed later by “+10 minutes | Pastry resting in freezer” and “45 minutes total”. Do not show an additional 45-minute jump after those 35 minutes. Show “At temperature | Oven ready” for a preheat of unspecified duration; do not invent a fixed preheat time.

### Repeated active work

Demonstrate the technique at normal speed first. Then label shortened repeated work **“Demonstration shortened — {actual duration or source range}”**. If the recipe gives no duration, use **“Repeated action shortened”** without inventing one. Resume at normal speed to show the endpoint. Keep speech at normal speed and use sound appropriate to the edited action. A shortened whisking demonstration is not a separate waiting interval.

### Parallel work and conditional checks

For overlapping tasks, use a status line, for example **“Blind baking: 45 of 60 minutes elapsed · 15 minutes remaining”**, while the host starts the filling. The filling demonstration belongs within those last 15 minutes. At the next transition, identify the cumulative baking checkpoint; do not count another full hour.

When a source gives a range or a doneness target, the depicted duration is one example, not a promise. State when checking begins, show how to check, and explain what to do if it is not ready. Any conditional demonstration is labelled **“If needed”** and explicitly rejoins the main method. Never imply that a timer alone establishes doneness.

Log every time jump and shortened action in the production brief. Title cards and dissolves count towards the 20-minute ceiling.

## Build the production package

Save a completed brief as `videos/{Recipe_filename_stem}.md`, preserving the recipe filename's capitalisation and underscores. Keep the recipe in `recipes/` unchanged unless separately asked to edit it.

The package needs three kinds of information in one file:

1. **Production specification:** source revision, facts, reference assets, character and voice, set, visual style, timing plan and continuity rules.
2. **Viewer sequence:** the actual film, in recipe order, with exact shot actions, dialogue, text and sound. The production specification is not spoken or shown as an opening chapter.
3. **Handoff and checks:** prompts, clip assembly, captions, chapter list, credits, description copy, coverage and unresolved dependencies.

Use this fill-in scaffold. Replace every placeholder in a completed brief; retain only applicable optional recipe sections. Expand the repeated shot block for all shots. A compact table is acceptable if it retains all the same information, including explicit defaults for inherited fields.

````markdown
# {Dish emoji} {Recipe Title} — video script and storyboard

## Production specification

- Source recipe: {repository path and permalink at commit}.
- Source revision: {commit SHA; date checked}.
- Supporting references: {template, glossary, style guide and component permalinks}.
- Destination: YouTube, 16:9, 1920 × 1080, 25 fps.
- Planned duration: {mm:ss, including graphics and credits; no more than 20:00}.
- Cooking-time summary: {copy the source summary verbatim; separate from video runtime}.
- Depicted path: {selected permitted option, conditional branches and illustrative timing}.
- Production choices: {handedness, vessel among supported choices, kitchen layout}.
- Unresolved source issues: {None, or the exact issue and consequence}.

### Source facts and coverage

| Source section / action | Exact fact or instruction | Shot IDs | Verification |
| --- | --- | --- | --- |
| {Ingredient or step} | {Amount, action, duration, temperature or endpoint} | {IDs} | {Where it is visible and/or spoken} |

### Reference assets and continuity

| Asset ID | Source file / permalink | Role | Fixed details |
| --- | --- | --- | --- |
| HOST-01 | {README WebP and glossary WebP} | Character | {Face, hair, outfit, hands, voice} |
| FOOD-01 | {Recipe WebP and written recipe} | Finished appearance | {Shape, colour, garnish, serving vessel} |
| SET-01 | {Written layout, plus derived reference when produced} | Kitchen | {Positions, lighting, equipment} |

{Copy the shared visual and voice instructions into this brief. List all
recurring props, ingredient states and practical safety staging, such as
oven gloves for hot trays. Distinguish references already supplied from
assets still to be generated.}

### Screen-time and process-time plan

| Sequence | Screen interval | Actual process duration / checkpoint | Parallel task or condition | Jump text |
| --- | --- | --- | --- | --- |
| {Sequence} | {mm:ss–mm:ss} | {Actual time or endpoint} | {None or exact overlap} | {Exact card wording or None} |

## Viewer sequence

### Introduction and summary

{Finished-dish preview, concise promise, exact recipe summary. Add shot blocks.}

### 📌 Before you start

{Source prerequisites and timings, with their demonstration or clear explanatory view.}

### 🔪 Equipment

{Source equipment and dimensions; visible working kit also accounted for in production props.}

### 🥕 Ingredients

{Copy every source group and ingredient quantity; specify the exact card pages.
Show the host introducing or measuring the ingredients, with preparation
assigned to explicit shots at the appropriate point.}

### 🍳 Directions

#### Step 1: {Exact source step title}.

##### {SHOT-ID} — {Action}

- Screen time: {start–end, duration; intervals include all transitions}.
- Source: {step and specific sentence/action}.
- Process time: {start/end checkpoint or normal-speed action; parallel work}.
- References: {asset IDs and preceding shot/end-state reference}.
- Camera: {shot size, angle, stable position or motivated movement}.
- Start state: {host, food, tools and their locations}.
- Visible action: {ordered hand movements, tool use and material change;
  identify normal-speed demonstration and any shortened repetition}.
- End state / continuity: {precise food and prop state carried to next shot}.
- Host dialogue, verbatim: “{Exact words, including helpful reason where relevant}”.
- Speech mode: {visible lip-sync / same host speaking over hand close-up / silence}.
- On-screen text, verbatim: {text, position, display interval; None if none}.
- Sound: {specific synchronised sounds; music rule; silence where appropriate}.
- Transition: {cut / exact time-jump wording and duration; no unmarked time change}.
- Acceptance check: {visible evidence of the action and endpoint; specific errors to reject}.

{Repeat for every shot and source step, preserving step order. Put each tip
where the host performs the relevant action. Include complete branches.}

### 📝 Notes and substitutions

{Source notes with exact dialogue, visual support and conditional labels.}

### 🫙 Storage and make-ahead

{Source storage durations and actions, with readable cards and demonstrations.
Make-ahead alternatives must not look like extra steps after serving.}

### 🔗 Used in

{For component recipes only, retain the source's links and brief screen treatment.}

### 🗺️ Origin

{Source country/region and concise history, with a short end-sequence treatment.}

### 🏷️ Tags

{Exact source tags and allergens. Repeat allergens earlier if useful; retain this position.}

### ✍️ Credits

{Recipe author/editors as published; adaptation attribution; licence and changes statement.}

### 📚 Sources

{Source recipe permalink, original source references retained as recipe provenance,
style/character references and any separately verified additions. Identify inherited
source references rather than claiming a fresh verification. Full links in description.}

## AI production handoff

{Global prompt; shot-prompt assembly; reference attachment plan; voice and sound;
graphics/captions; filenames; clip splitting and joining; exact chapter list and
ready-to-use YouTube description including source/credit/licence text.}

## Validation

{Coverage audit, measured dialogue fit, runtime sum, process-time audit,
continuity review, reference availability, unresolved issues and render status.}
````

## Tool-independent generation and assembly

Use the following as the master instruction, filled with the completed brief. Copy the shared instructions into the handoff so a new AI does not have to infer them from earlier chat messages.

```text
Create the video specified in the attached completed recipe brief.
Treat its source facts, exact dialogue, shot order, process timings and
acceptance checks as binding. Do not invent missing cooking steps, extra
ingredients, garnishes, quantities or new advice. Flag unresolved source
conflicts before production.

Create original animated oil-painting scenes with layered colour, visible
directional brushwork, translucent shadows, restrained warm earth colours,
cool blue-grey distance and selective highlights. Keep food naturally
coloured and clearly painted. Use coherent light and plausible scale.
Hands, tools and the food being worked must remain clearly readable.

Use the same man from the attached README WebP and glossary WebP in every
shot: curly dark brown hair, light stubble, cream rolled-sleeve shirt,
plain cream tied apron and dark trousers. Preserve his identity and the
locked kitchen layout. He performs every cooking action. Use a warm, calm
British male voice with upper-class Queen's English / Received
Pronunciation. Keep the language simple and the pace unhurried.

Generate each shot from its start state through the specified action to
its end state. Demonstrate new techniques at normal speed. Attach the
character, set, food and previous end-frame references relevant to it.
Do not replace cooking with a slideshow, magical transformations or a
montage of prepared ingredients. No extra fingers, changing utensils,
floating objects, hidden actions or food-state discontinuities.

Output clean 16:9 picture clips plus the specified voice and sound assets
where supported. Add exact quantities, temperatures, time-jump cards,
readouts and captions in editing, not as unreliable generated lettering.
Follow the brief's complete time-jump convention. Keep screen time
distinct from cooking time. The assembled film must not exceed 20:00.

If this tool cannot render video, return the production package and
prompts for a capable tool, clearly labelled as such. Do not claim a
video exists. Report only settings and asset identifiers actually used.
```

For each shot, build its prompt from **master instruction + character/set/food reference attachments + complete shot block + previous end state**. Resolve every reference ID to an attached image or explicit description. Do not send an isolated action such as “whisk” without its ingredients, vessel, amounts already added and intended texture.

If a service supports shorter clips than the editorial shot, split the shot into `S01a`, `S01b`, and so on at natural action boundaries. Specify each subclip's start and end state, share the previous end-frame, and allocate the shot's exact dialogue across subclips without dropping words. Use brief matching handles for editing, trimmed out of the final duration. Never squeeze a whole long recipe action into the model's clip limit.

Generate and check reference assets first, then a short representative trial showing the host, a hand technique, a time jump and a spoken tip. A downstream editor may revise generation prompts to correct failed visuals, but may not change the recipe. Render clips individually, check them, then assemble. Keep a record of prompt text, actual tool/model if reported, reference assets, output IDs and revisions. Tool-specific seeds or switches are optional, not part of the portable recipe specification.

Suggested downstream delivery set: the completed Markdown brief; named reference assets; numbered picture clips; separate host speech and effects where supported; edited film; captions in SRT or VTT; and the exact YouTube title, description and chapter timestamps. Example filenames: `S01_picture.mp4`, `S01_voice.wav`, `Recipe_title_final.mp4`, `Recipe_title.en-GB.srt`. These are intended outputs, not files that this template claims already exist.

For use in ChatGPT or another assistant, attach this template, the source recipe and reference images, and ask for the completed brief first. Then give that complete brief and assets to the chosen video workflow. Capability depends on the available tool; do not assume every chat can render or combine video.

## Final checks

- [ ] The brief records its recipe revision and can be understood outside the original conversation.
- [ ] Every ingredient, preparation verb, source step, temperature, wait, doneness cue, tip and conditional action maps to a shot. No missing peeling, chopping, rolling, pouring or handling is disguised by a cut.
- [ ] Quantities and terminology match the source. The host visibly measures or uses the specified amounts; spoon measures are level.
- [ ] The video sequence follows the recipe's section and step order; optional absent sections are omitted.
- [ ] Dialogue is fully written, fits a calm read-through and includes helpful reasons during the relevant work.
- [ ] All screen intervals are contiguous and sum to at most 20:00, including transitions, alternate demonstrations and credits.
- [ ] Every time jump has exact text and a process checkpoint; parallel waits are not added twice. Variable times are presented as examples with the source endpoint.
- [ ] Hand movements, contact, tool use and food transitions are visible and plausible. Decisive technique moments are normal speed.
- [ ] The character, outfit, voice, handedness, equipment and kitchen remain consistent. Shot prompts carry sufficient context when used separately.
- [ ] The painted style remains coherent while the working area, readouts and captions remain legible on a small screen.
- [ ] Source-specific serving rules are preserved: no unsupported garnish, incorrect vessel or steam from a cold dish.
- [ ] Full references, credits, licence and adaptation statement are in the handoff and YouTube description. Do not imply inherited external sources were freshly checked.
- [ ] Actual generated assets and settings are recorded separately from proposed assets. The final rendered film and captions are checked before claiming production is complete.

## Credits and sources

- **Original author:** [John-44](https://github.com/John-44), with AI assistance for this video adaptation template.
- [README](README.md): practical, precise, succinct cooking principles.
- [Recipe template](Recipe_template.md) and [Terminology glossary](Terminology_glossary.md): structure, language and measurements.
- [Illustration style template](Illustration_style_template.md), [README illustration](images/Readme_banner.webp) and [glossary illustration](images/Terminology_glossary.webp): painted treatment and recurring host.
- Owner's video brief: YouTube 16:9, no more than 20 minutes, visible step-by-step cooking, consistent labelled time jumps and a warm male Queen's English voice. Video composition and editorial overlays adapt the masthead conventions for teaching.

---

© 2026 [John-44](https://github.com/John-44). Licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
