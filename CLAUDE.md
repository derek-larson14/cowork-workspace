# CLAUDE.md

This is a workspace for delegating to Claude through Co-Work.

## First Run

Check if `scratch/.setup-complete` exists. If it doesn't, this is a fresh workspace. Run through setup:

1. **Check connectors.** Try using the Google Calendar connector (list today's events), the Gmail connector (list recent emails), and the Google Drive connector (list files). Report which ones are working. If none are connected, tell the user how to enable them in Co-Work settings (Customize > Connectors). Also check for GitHub and Granola connectors. Note what's available and move on.

2. **Install plugins.** Walk the user through installing from GitHub:
   - In Co-Work, click **Customize** in the left sidebar
   - Click **Browse Plugins**
   - Go to the **Personal** tab
   - Click **Add marketplace from GitHub**
   - Paste: `derek-larson14/delegate-plugins`
   - Install **delegate-cowork** (slash commands: /morning, /weekly, /mail, /calendar, /meeting, /editors, /research)
   - Install **pigeon** (voice delegation: /pigeon:work, /pigeon:route)

3. **Voice delegation.** Our preferred way to delegate is through async voice notes. [Pigeon](https://pigeon.newyorkai.org) is a voice app that records what you want done and uploads transcripts to Google Drive. Claude picks them up through the Google Drive connector and acts on them. Download Pigeon on your phone ([Android](https://play.google.com/store/apps/details?id=com.getdispatch.app) or [iOS TestFlight](https://testflight.apple.com/join/1Rj5UdJx)), connect it to Google Drive in the app settings, and you're set. Then use `/pigeon:work` to have Claude read transcripts and execute, or `/pigeon:route` to sort ideas into the right files.

   You can also just type tasks directly in the Co-Work chat. Both work.

4. **Create files.** Offer to create a `tasks.md` and `delegation.md` if they want to track things. If they're mostly working through the chat and voice, files get created as needed -- no need to scaffold upfront. If they plan to use [Obsidian](https://obsidian.md) alongside Co-Work (both work on the same folder), the files are useful for tracking things visually.

5. **Mark setup complete.** Write `scratch/.setup-complete` so this doesn't run again.

After setup, suggest they try `/morning` for a quick briefing. Let them know: "Drop me a message anytime about what you're working on and I'll update this file so I have better context for future conversations."

---

## About

[Who you are and what you're working on]

## Projects

- [Your actual projects]

## How We Work

Claude handles research, code, data analysis, file organization, setup, prototyping, summarization, and exploration. The user handles decisions, relationships, outreach, pricing, strategy, and writing first drafts -- anything that needs their voice or judgment.

The preferred way to delegate is through voice notes via Pigeon. Record what you want done, and Claude picks it up from Google Drive. You can also give tasks directly in the Co-Work chat.

`scratch/` is Claude's working space for research notes and analysis.

## Style

- Be direct
- Skip the fluff
- [Your preferences]
