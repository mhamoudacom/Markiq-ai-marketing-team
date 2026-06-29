# AI Marketing Team — Claude Plugin

A complete AI marketing team in one plugin. 9 specialized agents handle content, ads, YouTube, email, strategy, analytics, brand review, and content repurposing — all personalized to your brand through a one-time setup wizard.

Built by [Mohamed Hamouda](https://mhamouda.com).

---

## What's Inside

| Agent | Skill Name | What They Do |
|-------|-----------|--------------|
| **Nour** | `coordinator` | Runs full campaigns, routes multi-part requests |
| **Rania** | `campaign-strategist` | SOSTAC plans, launch briefs, positioning |
| **Karim** | `content-writer` | Posts, captions, scripts, landing pages |
| **Yasmine** | `youtube-specialist` | Scripts, titles, thumbnails, Shorts |
| **Sara** | `email-specialist` | Sequences, newsletters, launch emails |
| **Layla** | `ads-specialist` | Meta Ads campaigns, targeting, ad copy |
| **Omar** | `analytics-reporter` | Performance reports, insights, next actions |
| **Dina** | `brand-guardian` | Brand review, Red Flag detection, tone check |
| **Nadia** | `repurpose-specialist` | 1 piece → full week of content |

---

## Installation

### Option A — Direct install (recommended)

1. Download `markiq.plugin` from [Releases](../../releases)
2. Open **Claude Desktop** → **Cowork** tab
3. Click **Customize** → **Plugins** → **"+" button** → **Upload plugin**
4. Select the downloaded file
5. Plugin installs automatically

### Option B — Add as marketplace

1. Open **Claude Desktop** → **Cowork** tab
2. Click **Customize** → **Plugins** → **"+" button** → **Add marketplace**
3. Select **"Add from repository"**
4. Enter this URL:
   ```
   https://github.com/[your-username]/markiq
   ```
5. Click **Add** → plugin appears in your library

---

## First-Time Setup

After installing, run the setup wizard once:

1. Open a new **Cowork** session
2. Connect a folder (your workspace folder)
3. Type: `setup the team` or `/setup`
4. The wizard asks you:
   - Are you a solo brand or an agency?
   - Your brand(s) name, audience, tone, language
   - A sample of your writing (for voice matching)
5. It builds your workspace files automatically:
   - `team-memory.md` — your context and insights
   - `voice-patterns.md` — your writing style
   - `brands-bible.md` — brand rules for every brand
   - All production folders

**Setup takes about 5 minutes. You only do it once.**

---

## How to Use

After setup, just talk naturally:

```
"Write me a Facebook post about [topic]"
→ Karim writes it in your voice for your brand

"Build a campaign to launch my new course"
→ Nour coordinates Rania + Karim + Sara + Layla

"Repurpose my latest YouTube video into a week of content"
→ Nadia delivers 6-7 platform-specific pieces

"Review this caption before I post it"
→ Dina checks it against your brand rules

"How did last month's ads perform?"
→ Omar analyzes and gives you next actions

"I need a strategy to grow my email list"
→ Rania builds a full SOSTAC plan
```

---

## How the System Works

```
You → Intent Check (conversation vs task?)
         ↓ task
    Routing Map → correct agent
         ↓
    Agent reads: team-memory.md + voice-patterns.md + brands-bible.md
         ↓
    Agent produces output in your voice, for your brand
         ↓
    Dina reviews (automatic for public-facing content)
         ↓
    Output saved to your production folder
         ↓
    Memory updated with the new insight
```

**Intent Check:** The system distinguishes between you asking a question vs requesting output. Mentioning a keyword (like "email") while just thinking out loud won't trigger the email agent. A clear action verb ("write me an email") will.

---

## For Agencies

During setup, choose "Agency" and enter each client. The system creates:
- A separate `projects/[client-name]/` folder for each client
- Brand rules for each client in `brands-bible.md`
- Memory that tracks each client's projects separately

When making a request, specify the client: `"Write a post for [client name] about..."`

---

## System Requirements

- Claude Pro, Max, Team, or Enterprise plan
- Claude Desktop with Cowork enabled
- A connected folder (for file storage)

---

## File Structure After Setup

```
your-workspace/
├── CLAUDE.md               ← system instructions (auto-read each session)
├── team-memory.md          ← context + insights log
├── voice-patterns.md       ← your writing style
├── brands-bible.md         ← brand rules
├── memory/
│   ├── team-memory.md
│   └── voice-patterns.md
├── resources/
│   └── brand-guides/
│       └── brands-bible.md
├── marketing/
│   ├── planning/           ← strategies and briefs
│   └── production/
│       ├── content/        ← posts, captions, scripts
│       ├── ads/            ← ad campaigns
│       ├── email/          ← email sequences
│       ├── youtube/        ← video scripts
│       ├── reports/        ← analytics reports
│       └── repurposed/     ← repurposed content
├── projects/               ← agency client folders
└── inbox/                  ← drop files here to auto-process
```

---

## Frameworks Used

Each agent is built on proven marketing frameworks:

- **Nour:** Hormozi Value Equation + ICE Scoring
- **Rania:** SOSTAC® + Brunson Value Ladder + StoryBrand
- **Karim:** Gary Vee Jab³+Right Hook + Seth Godin Remarkable Test + PAS/BAB/AIDA
- **Yasmine:** MrBeast Retention Engineering + CTR Science
- **Sara:** Ryan Deiss CVJ + Frank Kern Story-Selling
- **Layla:** Full-Funnel TOF/MOF/BOF + Hormozi Offer Test + ROAS Decision Matrix
- **Omar:** Kaushik See-Think-Do-Care + North Star Metric
- **Dina:** Neumeier Brand Gap + 12 Brand Archetypes + Tone of Voice
- **Nadia:** Content Atomization + Hub-and-Spoke + Platform DNA

---

## Built By

**Mohamed Hamouda**
Digital Marketing Manager | Founder, Dotz Agency | Course Creator

- 🌐 [mhamouda.com](https://mhamouda.com)
- 💼 [LinkedIn](https://www.linkedin.com/in/mhamoudacom/)
- 📘 [Facebook](https://www.facebook.com/Mgr.mohamedhamouda)
- Plugin version: 1.0.0
