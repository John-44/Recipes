# Agent instructions

![Oil painting of a butler giving instructions to a robot, with other robots farming in the background](images/AGENTS.webp)

This repository holds recipes for UK home cooks, written in Markdown. There's no code to build or test: the work is writing, editing and reviewing recipes, to the standard these files set:

- [Recipe_template.md](Recipe_template.md) says how every recipe is written, from file names and sections to credits and sources, and ends with a checklist.
- [Terminology_glossary.md](Terminology_glossary.md) pins the exact words the recipes use.
- [Declined_suggestions.md](Declined_suggestions.md) lists suggestions that have already been turned down.
- [recipes/](recipes/) holds the recipes, one per file.

Every rule about what goes in a recipe and how it's written is in the template or the glossary. This file covers how to work in the repository, and doesn't repeat them.

## Before you begin

- Make sure you're working from the latest `main` on `origin`: fetch it, and bring your branch up to date if `main` has moved. Several agents work here at once and their pull requests are often merged within hours, so a copy goes stale quickly, and work done on a stale copy can repeat changes already made or conflict with them.
- If your working folder contains `.claude/worktrees/`, leave it alone. It holds other agents' copies of the repository, so searching it turns up duplicate recipes and editing it changes their work.
- Read the template and the glossary in full before you create, edit or review a recipe, or change either file. Their rules are spread across many sections, and a recipe has to follow all of them.
- Read `Declined_suggestions.md` before you suggest a change.

## Making changes

- Keep each change to what the request needs: the change itself, and the updates it forces elsewhere. Leave the rest of the wording as it is. Every line has been reviewed, and rewording one can break a glossary term or a cross-reference. If you notice something else worth changing, suggest it at the end of your reply.
- When the user gives you exact wording, use it exactly as given, because they chose those words. Then check it against the glossary, especially the **Short name** and **Don't use** columns, and if it clashes, say so and offer a fix rather than changing it yourself.
- Keep the files consistent with each other. A rule changed in the template applies to every recipe, a component recipe's batch size has to match what the recipes that use it ask for, and the template and glossary quote recipe lines as examples. Search the repository for anything you change, and update whatever depends on it in the same pull request.
- Before you finish, read through your diff to check that it changes only what you meant it to.

## New recipes

- Check `recipes/` and the glossary's recipe titles first. If a recipe already covers the dish, or a note in one does, such as **Chicken instead**, say so and ask whether to build on it before you write a separate recipe.
- Ask about anything the user hasn't settled that would change the whole recipe, such as which version of the dish they want. Make smaller calls yourself, and list them under **Worth checking**.

## Recipe images

- Creating an image for a recipe is a separate step from writing or editing the recipe. Only do it when the user explicitly asks you to, even for a recipe you've just written.
- When they ask, read [Illustration_style_template.md](Illustration_style_template.md) in full and follow it.

## Checking sources

Some recipe sites block automated requests but still open in an ordinary browser. If a page won't open with your usual web tools, open it in the user's own Chrome through a browser extension such as Claude in Chrome, if you have one, and read it there.

If you still can't open the page, you can ask the user for assistance with opening the page, and if you still have difficulty you can give the user the URL and ask the user to print a pdf of the page for you.

## Questions and reviews

When the user asks a question about a recipe, answer it, and make no changes unless they ask for one.

When they ask for a review of a recipe, the template or the glossary, the deliverable is a numbered list of suggestions, not edits. Check it against the template, the glossary and the other recipes, check the cooking itself (technique, timings, amounts and food safety), and check that each source still backs what it's credited for. Give each suggestion its reason and the exact new wording, so the user can pick by number, and change nothing until they've picked. Then make only the changes they picked, and in the same pull request add the ones they didn't pick to `Declined_suggestions.md`, unless they asked to come back to them.

## Commits and pull requests

- Write commit messages, pull request descriptions and replies in plain British English. When you mention something the glossary lists, use its term.
- Start each commit message and pull request title with a verb, and say what changed, as in "Crack the coconut milk in Thai Yellow Prawn Curry".
- In a pull request description, say what changed in each file, quoting the new wording where the exact words matter. Then list under **Worth checking** anything you weren't sure about, couldn't verify or left alone on purpose, leaving it out if there's nothing. End by saying whether the credits changed, and why.

## Keeping this file current

If the user corrects how you work in a way that would apply to later tasks, offer to add it here, so every agent picks it up. Rules for the recipes themselves belong in the template or the glossary instead.

---

© 2026 [John-44](https://github.com/John-44). Licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
