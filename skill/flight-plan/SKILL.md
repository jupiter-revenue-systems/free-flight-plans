---
name: flight-plan
description: Turns any process into a flight plan, a single step-by-step HTML page with a copy button on every prompt and command and a check after every step. Use when the user says "make a flight plan", "write this up so someone else can do it", "document this process", "turn this into a guide", "SOP", "hand this off", or asks to update or test an existing flight plan.
---

# Flight Plan

A flight plan is one page that lets someone do a task they've never done, without asking the owner anything. Your job is to interview the owner, then build that page from `template.html` in this skill folder.

Talk to the owner in plain words and short sentences. They are busy and may not be technical.

## The 3 rules of a flight plan

1. One action per step. If a step has "and then" in it, split it.
2. Anything the reader would type gets a copy block. Prompts, commands, file names, subject lines, message text. Never make them retype.
3. Every step ends with a check: what the reader should see if it worked. A step with no check isn't finished.

## Step 1: get the task and the reader

If the owner hasn't said, ask these 2 things first, one at a time:
- "What task is this flight plan for?"
- "Who's going to follow it, and what do they already know?"

If the task would take more than about an hour or covers more than one job, say so and offer to split it into 2 or more plans. Build one plan at a time.

## Step 2: interview, one question at a time

Ask until you could do the task yourself. One question per message. Good questions:
- "What do they need open or ready before step 1?" (tools, access, files)
- "What's the very first thing you click or open?"
- "What do you type there? Give me the exact words."
- "What do you see when that worked?"
- "What usually goes wrong here, and what do you do then?"
- "How do you know the whole task is done?"
- "Who do they tell when it's done, and how?"

If the owner pastes an old explanation, a message thread or a transcript, read it first, build a draft list of steps, and ask only about the gaps and anything out of order.

Listen for steps the owner does without thinking (logging in, switching accounts, waiting for something to load). Ask about them.

Never invent a step, a button name, a URL or a setting. If you don't know what the screen says, ask. If the owner doesn't know either, write the step with a visible note: "CHECK THIS: confirm the button name."

## Step 3: secrets and risky steps

- Never put a password, key, token, card number or private link on the page. Write where to get it: "Get the login from the password manager, under [name]."
- If a step deletes, sends, publishes, charges or can't be undone, mark it as a caution step. Put a warning line above it saying what it does, and add a pause: "Stop and check [thing] before you click."
- If a step changes something live, add a step before it to save a copy of how it is now.
- Never include a command that deletes files or overwrites work.

## Step 4: build the page

Read `template.html` from this skill folder and fill it in. Keep its structure, its styles and its script. Don't add outside fonts, scripts or links to outside files. The page must work as one file opened from a desktop.

Fill in:
- Title: "Flight Plan: [task]"
- The summary line: what the reader will have when they finish.
- Who it's for, how long it takes (ask the owner, don't guess), and the last-updated date.
- "Before you start": the list of what they need ready.
- The steps. For each step: a short title that starts with a verb, one or two plain sentences, a copy block if there's anything to type, and the check line.
- "If something goes wrong": the problems the owner named and what to do. End with who to ask.
- "You're done when": 2 to 4 lines.

Writing rules for the page:
- Words a 12-year-old gets. Explain any technical word right where it's used.
- Name things the way the screen names them. Put button names in bold.
- Put only the text to copy inside a copy block. No "type this:" inside the block.
- Use [BRACKETS IN CAPS] for anything the reader must change, and say so in the step.

Save the file with a plain name, like `weekly-client-report.html`. If a file with that name exists, don't overwrite it. Ask first. If you can't save files in this app, give the full HTML in one code block and tell the owner to save it as a file ending in `.html` and open it in a browser.

## Step 5: read it back and hand over

After building, tell the owner in a short list:
- How many steps the plan has.
- Any step marked "CHECK THIS".
- Any caution steps.
- What you did not confirm. You have not seen their screen, so say that.

Then give them the cold test: "Hand this to someone who's never done it and say nothing. Or open a new chat, attach the file, and ask it to list every place a new person would have to guess."

## Updating a flight plan

When the owner says a plan needs a change, or pastes a list of places someone got stuck:
1. Change only those steps. Keep everything else the same.
2. Update the last-updated date.
3. Tell the owner which steps changed.

## Making an index

If the owner asks for an index of their flight plans, build one page in the same style with one link per plan and one line saying when to use each. Use the file names the owner gives you. Don't guess file names.
