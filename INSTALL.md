# How to install the Flight Plan skill

A skill is a small folder with instructions inside. Claude loads it when you say the right words. You install it once.

The skill is the folder `skill/flight-plan/`. It has 2 files in it: `SKILL.md` and `template.html`.

Menus move around as Claude gets updates. If a button isn't where these steps say, look for the word "Skills" in Settings.

## Claude.ai (the website or the desktop app)

1. Zip the `flight-plan` folder. On a Mac, right-click the folder and choose Compress. On Windows, right-click, then Send to, then Compressed folder.
2. In Claude, open Settings.
3. Find Skills. It's usually under Capabilities. If you don't see it, check that code execution and file creation are turned on, and that your plan includes skills.
4. Choose to upload a skill and pick `flight-plan.zip`.
5. Make sure the skill is switched on.
6. Open a new chat and type: `make a flight plan`. If Claude asks what task it's for, it's working.

## Claude Cowork

1. Open the Claude desktop app and go to Settings, then Skills.
2. Upload `flight-plan.zip` the same way as above, and switch it on.
3. Start a Cowork task in the folder where you'd like your flight plans saved. Type: `make a flight plan`.

## Claude Code

1. Copy the `flight-plan` folder into the skills folder in your home directory. This command does it from inside the download folder and doesn't overwrite anything that's already there:

```
mkdir -p ~/.claude/skills && cp -Rn skill/flight-plan ~/.claude/skills/
```

2. To use it in only one project, copy it into that project's `.claude/skills/` folder instead.
3. Start a new Claude Code session and type: `make a flight plan`.

## Using ChatGPT, or a plan with no skills?

You don't need the skill. Start a new chat, attach `SKILL.md` and `template.html`, and say: `Follow SKILL.md. Make a flight plan for: [your task].`

## Check it worked

Say: `Make a flight plan for making a cup of coffee. The person following it has never done it.` You should get a few questions, then one HTML file. Open it in your browser and click a copy button.
