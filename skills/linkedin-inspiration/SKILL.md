---
name: linkedin-inspiration
description: Browse LinkedIn profiles from the FLG swipe file for post inspiration. Use this skill before writing a LinkedIn post for Timotheus Yuen (FLG) whenever you want fresh angles, hooks, or topic ideas. Triggers on any mention of "competitor research", "inspiration", "swipe file", "what are others posting", or at the start of the daily FLG LinkedIn post generation workflow.
---

# LinkedIn Inspiration Research

Before writing today's LinkedIn post, browse 3 profiles from the FLG swipe file and extract what's working — hooks, angles, formats, CTAs. Use it as inspiration, never to copy.

## Step 1 — Read the Swipe File Dashboard

Use the WebFetch tool to load the FLG swipe file dashboard from GitHub:
`https://raw.githubusercontent.com/jasonlau70/flg-app/main/linkedin/index.html`

Parse the `DEFAULT_PROFILES` JavaScript array from the file. Each entry has:
- `name`: creator's name
- `url`: their LinkedIn profile URL
- `tag`: "cpa", "broad", or "both"
- `notes`: any observations already saved about their content style

Extract the full list of profiles from this array.

## Step 2 — Pick 3 Profiles

Randomly select 3 profiles from the list. Vary the selection each day — don't pick the same names repeatedly. Always mix at least one CPA/accounting-specific creator (tag: "cpa") with at least one broader business/entrepreneurship creator (tag: "broad" or "both").

Use the `url` field from each profile to navigate directly to their LinkedIn page — no need to search.

## Step 3 — Browse LinkedIn

For each of the 3 profiles, use Claude in Chrome to:
1. Navigate directly to their LinkedIn URL from the swipe file
2. Scroll to their recent posts section
3. Read 3-5 of their most recent posts

If LinkedIn requires a login, the user's browser session should already be logged in. If a profile is inaccessible, pick the next one from the list.

## What to Extract From Each Post

For each post you read, note:
- **Hook**: How does it open? (bold statement, question, story, stat, contrarian take)
- **Topic**: What's the core subject or angle?
- **Format**: Short and punchy vs long narrative, prose vs fragments
- **CTA**: How does it end? What question or action does it drive?
- **Why it works** (or doesn't): One sentence observation

## Step 4 — Write the Inspiration Brief

Synthesize what you found into a short brief. Keep it concise — this is a starting point, not a report.

Format:

---
**Inspiration Brief — [Today's Date]**

Profiles checked: [Name 1], [Name 2], [Name 3]

**Angles/themes worth exploring today:**
- [observation or topic angle you saw that could apply to Tim's content]
- [another one]

**Hook formats that stood out:**
- [description of a hook style or specific opener that worked well]

**One post worth noting:**
"[Paraphrase one post that was particularly strong and explain briefly why it worked]"

**What to skip today:**
[Any patterns that felt overused, corporate, or off-brand for Tim]
---

## Step 5 — Hand Off

Pass this brief directly into the LinkedIn post writing workflow. The post writer should use the brief as loose inspiration — borrowing angles or formats if relevant, ignoring if nothing fits. The goal is to stay aware of what's working in the space, not to mirror anyone else's content.
