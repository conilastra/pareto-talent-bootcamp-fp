---
type: source
source_type: transcript
title: Pareto Bootcamp Day 3
captured: 2026-10-03
origin_url: https://drive.google.com/file/d/1eDiX9eRzKkxmLoDq6q3Ve34qIRysuoa2/view?usp=drivesdk
slides_url: https://docs.google.com/presentation/d/1oIG9A8J6ZnBNZEAZ63iQiJ8JIrvUIZ9-ouzqpd6yVQg/edit
speakers: [Ivan Bunin, Amparo Linares, Gaspar Duarte, bootcamp participants (Q&A)]
tags: [bootcamp, day-3, second-brain, context-layer, action-layer, moc, frontmatter, wikilinks, morning-brief, daily-extract, access-trust, right-hand, delegation, proof-points]
status: draft
---

# Pareto Bootcamp Day 3: Second Brain Systems

> Distilled from the Day 3 slide deck (`Pareto_Bootcamp_Day3`) and the full Zoom transcript (`Pareto_Bootcamp_Day3 - Transcript.txt`, read in full). Both files are titled Day 3. Presenter: **Ivan Bunin** (Pareto Talent CEO). Amparo Linares ("Ampi"/"Amp") handles bootcamp ops and recordings; Gaspar Duarte answers chat questions. Session given live (Ivan references being in **Montevideo**). Audience: LatAm candidates training to become Right Hands. The transcript auto-captions render "Claude" as "Cloud/Clot/Clod", "Fathom" as "Fatim", "Kasim Aslam" as "Casi Maslam"/"Casim"/"Cassin", "Plaud" as "plot/PLOD", "wikilinks" as "Vicky/weekly links".

Related: [[bootcamp-day-1]] · [[bootcamp-day-2]] · [[bootcamp-day-4]] · [[right-hand-program|Right Hand Program]] · Second Brain Workshop · Morning Brief · Pareto Talent company facts

## Topic of the day
How to turn a founder's scattered context into a **Second Brain**: a structured folder of markdown files (context layer) plus live connectors (action layer) that Claude reads and writes. Reframed for Right Hands: building one **for a founder**, not for yourself, then running it daily (daily extract + Morning Brief). This is the same method Pareto sells to founders in its paid Second Brain workshop.

## Session outline (slide agenda)
1. The two-layer system: context and action
2. Why the files live in Drive, not in Obsidian
3. How Claude actually finds things: frontmatter, links, MOC
4. Building one for a founder, not for yourself
5. The Morning Brief, the daily routine, and what breaks

Actual flow: recap of Day 2 ("context rules") -> context sources -> access & trust -> architecture whiteboard -> Obsidian / frontmatter / wikilinks / MOC -> live build in Claude Code with the reverse-interview prompt (answered live with Pareto's real company data) -> Q&A -> populating context (YouTube interview, SOP PDFs, contractor agreement, Fathom, GoHighLevel transactions, Plaud/Omi wearables) -> routines/daily extract -> Ivan's Telegram assistant + voice agent demo -> six failure modes -> homework -> Q&A. Next day (Day 4): agentic workflows and automations; Friday: GoHighLevel + AI/CRM; next week: marketing, image/video generation, inbox management.

## Core thesis (slide: "The thing Ivan says most")
- "Context is what rules now."
- "Whoever had the best prompt was winning in 2022. Right now, whoever has the best context is winning."
- "AI is a force multiplier of people and of context. It is not its own input. It still needs both."
- "The problem with most founders is that their context lives in their head, which makes them the bottleneck."
- "Your job is to get that context out of their head and into something that outlives the conversation."
- Ivan: "a lot of people still will tell you, yeah, you need… you just need a better prompt. Which is wrong."

## Frameworks taught

### 1. The Two-Layer Second Brain (Context + Action)
- **Context layer** = static knowledge: SOPs, company history, contracts, the offer, strategy docs, books/podcasts. "This is what makes Claude sound like it knows the business, not like it's guessing." Physically: "just a folder" (Google Drive folder synced locally).
- **Action layer** = live connectors: Gmail, Calendar, Slack, Fathom, Notion, CRM, Stripe. Via native connectors, MCP ("Model Context Protocol") or API. "Some connect natively inside Claude, some need a custom MCP built for them." Ivan: ~85% of apps on the internet can be connected to AI.
- Analogy (slide): "Context without action is a filing cabinet nobody updates. Action without context is a assistant with amnesia, connected to everything and understanding none of it."
- Interface: Claude (Claude Code desktop preferred) reads the folder + connectors; outputs often as **Artifacts** ("pages or small apps... reports, KPIs, analysis, overviews, morning briefs"; preferred over PDFs/docs).
- **Context multiplication**: AI can pull from the action layer (Gmail, CRM, Stripe) and write distilled knowledge back into the static folder. "It's not happening by default... if you connect a Gmail... it's not like Claude immediately knows everything about your email." Needs a routine.

### 2. Six context sources worth extracting first (slide "Context, in practice")
1. **SOPs and process docs**: "If it isn't written down, that's your first thing to document, not skip." Ivan: "if you do something twice, then there should be a SOP for that." SOP = standard operating procedure, "a written tutorial for somebody... that somebody else will be able to follow." Example shown: Pareto's internal SOP for judging bootcamp final projects (announcement on last day, written instructions via Slack, agenda, requirements, scoring rubrics and score meanings).
2. **Company and founder history** (incl. org charts so AI knows who does what).
3. **Contracts and the offer**: "So Claude never invents a number that isn't true." What we promise clients, what we promise Right Hands, terms, violations.
4. **Strategy docs**: quarterly/annual goals, strategy sessions ("amazing sauce for AI").
5. **Books, podcasts, interviews**: "Often the richest source, and usually the most ignored."
6. **Call transcripts and client language**: from Fathom; "When Claude drafts an email or an ad, it reuses what actually converts."

### 3. Access is earned, not assumed (trust staging)
Slide rules: a founder connecting their own Gmail is a different act of trust than handing it to a Right Hand "they met last week"; ask only for what the current task needs; document access in plain language "the founder could read in ten seconds"; anything touching money, passwords, client data follows the Day 2 rule ("Never paste it anywhere outside what you were explicitly given"). "Every connector you add is a decision the founder has to trust you made correctly."
Staging:
- **Week one (Days 1-7)**: read-only, task-scoped, a shared Drive folder; nothing that can send, delete or spend. Ivan: ask for an export or screenshot instead of CRM access.
- **As trust builds (first 30 days)**: broader read access; write access to things you maintain (e.g., the Second Brain folder); Gmail, more materials.
- **Only when asked (Days 30+)**: client-facing, financial, irreversible ("being able to send email to 30,000 people").
Pitch technique: give the reason + promised result ("Now this is a trade"). Example ask: Gmail access so I can extract emails into the second brain, get you to inbox zero, and leave you only emails marked as tasks. Frame limited access as limiting proactivity: "if you want me to be more proactive... pick up a project and run with it without asking you every single question, then I need to have a full perspective."

### 4. Architecture: local Drive folder + Obsidian as window
- Install **Google Drive desktop** so the folder is local; Claude Code reads/writes "at full local speed, with none of the rate limits a live API connection would hit"; Drive syncs to cloud for founder/team. (OneDrive etc. also work; a plain local folder is fine if not shared.)
- Analogy: "working from a document on your own desk" vs "requesting a new copy from a shared cabinet every time."
- **Obsidian** "is the window, not the building." "Obsidian does not store anything." "Obsidian is the dashboard in a car. The engine runs whether or not you're looking at the dashboard." Ivan: "it's not Obsidian second brain. It's a ridiculous term, because second brain is just a list of Markdown files." Optional; used for preview, navigation, graph view (open folder as vault).
- Markdown is "the best format for AI." Whole Pareto brain ~200 MB because it's all text.

### 5. How Claude finds things: Frontmatter, Wikilinks, MOC (4 hops)
- **Frontmatter**: "a quick table... in the beginning of the file, that explains what this file is" (category, created/updated date, version, active/archive status, audience, related links). Lets AI understand a file without reading it, saving tokens. Written automatically by AI.
- **Wikilinks**: links between files (e.g., marketing file links the sales file; an interview note links to the "EA interview SOP"; ICP doc links). Purple links in Obsidian; white lines in graph view.
- **MOC (Map of Content)**: one per folder, "a short index explaining what's inside", built automatically by AI. Analogy: "A library card catalog."
- Four hops (slide): **Enter the folder -> Read the MOC -> Open the file -> Follow a link** ("Four hops, not one giant read").
- **CLAUDE.md** at the root tells Claude to treat the folder as a second brain, convert dropped docs to markdown and file them; also guards against polluting it ("without a specific prompt, do not populate the second brain").
- Why it compounds (slide): "It remembers things nobody thought to search for." "Unlinked notes are context that might as well not exist." "Link as you write. Never plan to link everything later." Maintenance: occasionally ask AI to interlink everything / check for orphaned files (monthly routine or manual; Ivan has done it twice).

### 6. Building one for a founder: the Reverse Interview
- Slide: "You can't dictate someone else's business." Founder-facing build starts with the founder talking ~45 minutes. "The founder-facing workshop calls this a reverse interview. You are conducting one, not sitting for one." "Skipping this step is why a Second Brain sounds like nobody in particular."
- Two routes: **Structured intake call** (book 30 minutes specifically; section by section: identity, offer, team, people, tools; record in Fathom) or **Mining existing material** (sales/onboarding calls, website-to-markdown, Fathom; "faster when it exists, but it never fully replaces asking directly"). Ivan: answering questions is easier for founders than explaining unprompted; can be done as interview for founders uncomfortable opening Claude.
- Pareto has two prompts: one for **the company** (Second Brain Workshop prompt) and one for **the entrepreneur as a person** (multiple businesses, other commitments). Takes 10-15 min if experienced, ~1 hour otherwise. "You cannot build a template for a second brain. Because each second brain will be unique."
- Live build output: (1) folder design (top-level: context, company, departments; sub: strategy, decisions, commitments...), MOC per folder; (2) file templates (company identity, morning brief instructions, clients) with frontmatter and links; (3) source-material extraction queue / to-do list. Build created 71 folders and ran ~17 minutes.
- **Librarian, never the shelver** (slide): feed raw material in and tell Claude to file it; "Never drag a file straight into a structured folder yourself"; "The moment a human starts manually organizing the folders, the structure starts drifting." Even raw transcripts go in through Claude.
- When to split brains: by **who needs access**. Default "one second brain for one company"; separate personal (taxes, residencies, travel) from business; split departments if access must differ. Within Pareto each Right Hand works with one entrepreneur.
- Sessions: many sessions can share the same context folder ("all of them are grounded in one rooted truth"); long sessions -> compact or write a **handover document** into the brain. Multiple brain folders can be attached to one session (read, not written by default).
- Keep vs discard: don't delete old context ("you never know what will be useful"), but don't feed trash: "80% of the emails are spam."

### 7. Running it day to day: Daily Extract + Morning Brief
- **Daily extract** (slide): check Slack, Fathom, Gmail and the founder's dictation every day; pull out promises, decisions, anything that reads like a task; "Every single item traces back to where it came from. A promise with no source is just a guess." Same discipline as the Day 1 EOD report. Ivan's runs as a scheduled routine at **8 A.M.** across Slack, Fathom, Plaud, Gmail, iMessage, writing to the second brain and the CRM database.
- **Morning Brief** (slide "now for someone else to read"): 1) what they committed to; 2) what's blocked and what's blocking it; 3) what has to ship today, "ranked, not just listed"; 4) context for every meeting on today's calendar. "You are the one who has to know if it's wrong before the founder ever sees it."
- **Retrieval test** (before calling it done): ask something real you already know; check it found the right file, "not just whether the answer sounded plausible"; "If it can't find something you know is in there, the structure is wrong. The model is not the problem." "A Second Brain nobody has tested is a folder with good intentions."
- **Build it so it survives you**: top-level README in plain language; note anything unusual about the founder's setup; "The measure of a well-built Second Brain is whether the next Right Hand can pick it up cold." "You were hired to make yourself replaceable in the best sense, not indispensable in the worst one."

### 8. Six ways a Second Brain goes wrong (slide)
1. **Connected, not briefed**: action layer works but no context fed (Ivan: connectors connected but never pulled from).
2. **Broken navigation**: missing frontmatter or MOC; "Looks like Claude forgot everything. It just can't find the file." Fix: ask AI to analyze structure for orphaned/broken files.
3. **Manual filing**: human drags files; "structure drifts within a week."
4. **Notes that never got linked**: "Functionally invisible."
5. **One brain, two audiences**: personal and business mixed, then shared.
6. **Access never revoked**: teammate/connector keeps permissions after losing relevance.
"None of them are the model's fault."

### 9. Ivan's Claude personal-preferences prompt (shared on request)
Personality profile so Claude knows his weaknesses; communication style: "lead with the answer, recommendation, or diagnosis... be direct and confident. No affirmations, like, great question, absolutely, certainly. Short, dense paragraphs. Push back when I'm wrong or something's missing, don't over-soften hard truths, no emotional cushioning."

### 10. Claude Code permission modes (as taught)
Auto, Manual (approve every change), Accept edits, Plan ("preferred mode whenever you're just starting a bigger project"), Bypass permissions (used in demo). Use standard/cheaper models; ignore model-cost noise. Git install needed once (Zoom tutorial link shared).

## Proof points & numbers
**Pareto company facts (dictated live by Ivan into the intake):**
- Legally registered in **Arizona**. One-liner: "this company finds. Trains, places, and manages, executive assistants from Latin America with entrepreneurs from the United States."
- "already mature, about **3 years old**, and approximately **$3 million annual recurring revenue**."
- 12-month objective: "get to **300 placed right hands**. Right now, we are at **100**."
- Model: places Right Hands, "acting as **employer of record**. The Bootcamp is free, it's a training and recruitment model. And the primary revenue model is the **monthly retainer**."
- ICP: "small and medium businesses in the United States. Primarily **founder-led companies**. Usually making at least **$500,000 a year**. Typical sales cycles is approximately **2 weeks**."
- Headcount ~**15 employees**, ~**250 contractors** (about 100 are placed EAs).
- Departments: Client Success Management (Rita Barisha), Sales (Christian), Marketing (Ivan), Ops (Virginia), Finance (Juan Cruz). Gaps: need stronger sales and marketing departments.
- Leadership: Ivan Bunin (CEO), Kasim Aslam (co-founder).
- Key accounts: **Joe Polish (Genius Network)**, **Justin Donald (Lifestyle Investor)**, "a lot of other prominent entrepreneurs." No investors; advisors e.g. **Greg Smith**.
- Cadence: Monday trainings for EAs, Friday office hours; weekly reporting on sales, placements, social media numbers; no formal framework.
- Tool stack: Google Workspace (Gmail, Calendar, Drive), Slack, Google Meet, Notion (PM), **GoHighLevel** (CRM), Stripe (finance), Wise/Payoneer/Gusto (HR/pay), Predictive Index; Shortwave (inbox); Fathom; website "vibe-coded" with AI.
- Biggest thing in Ivan's head: marketing; 6-month goal: Claude as full assistant for the whole company.
- Pareto teaches founders delegation: "We are spending **90 minutes every single Friday** teaching them on how to let go."
- Pareto acts as "a sort of **guarantor**" so clients trust placed Right Hands with access.

**Second Brain offer proof:**
- "6 sessions on teaching people how to do second brains, teaching entrepreneurs, and we are charging **$100 per seat**... so far we've trained maybe **300 entrepreneurs**."
- Gaspar has done ~**15 build-outs**; "we charged entrepreneurs **$500** for each... we could have charged probably, like, $2,000, maybe $3,000."
- "this is proprietary... I don't think anyone else is doing that."
- Every placed EA who tried finished the build: "I haven't had a single person who wasn't."
- AI cost: of 100 placed people, none caused a credit problem; Pareto team spent **$580** extra this month on top of ~10 subscriptions (~$1,000 total); Ivan downgraded Max from $200 to $100/month.

**Other stats:**
- "A 2014 study of 350 entrepreneurs found the average founder is running about **14 different systems** in their head at once, unlabeled and disconnected." (14 -> 1 Second Brain)
- Ivan's clip with Kasim got **10x median views** on Instagram (19 saves vs median), surfaced by his AI assistant.
- Ivan's Pareto brain: ~**200 MB**.
- Ivan: "VAs will be replaced at mass, at bulk, by AI within this year, probably."

## Stories (2-4 lines each)
- **Caro babysitting**: a client/contact named Caro mentioned on a call she'd babysit for Ivan. When he later scheduled a Buenos Aires trip, AI surfaced that she's in Buenos Aires and offered. Power of links: "it linked Caro to Buenos Aires."
- **Juan Cruz retrieval**: Ivan texted his Telegram assistant "what did Juan Cruz ask me for?" It checked Fathom and the brain and answered: $70,000 to pay salaries plus invoice confirmations.
- **Voice agent "deep work" demo**: voice assistant walks Ivan's task list (Second Brain workshop fulfillment audit before relaunch; Juan Cruz fixing checkout so the 3% card fee isn't applied to ACH), creates follow-ups and checks Slack.
- **Two years ago, I started as your executive assistant**: a YouTube interview audio played during demo (Pareto/Kasim content): "Two years ago, I started as your executive assistant checking your emails, and now we have… three… One with an 8-figure valuation." (Partial, audio cut; speaker not identified.)
- **Bootcamp evolution**: Ivan used to teach EAs to build GoHighLevel sites by hand; now "you will open your Claude and say, hey, change it to blue." Pareto's site is AI-coded; blog posts are generated from yesterday's conversations, in his voice, auto-indexed in Search Console.
- **AI-run LinkedIn**: posts and images created and published by AI via Social Planner without Ivan doing anything.
- **Hotel confirmation number**: why you shouldn't under-populate the brain.

## Founder pain language & objections (verbatim)
- Founders withholding Gmail: "belief number one is that, hey, like, you will not have the full context, you will not know how to reply, and second is you don't have my voice, you won't be able to write like me." -> "These two things we are fixing with the second brain."
- "in the majority of cases, this is their, like, baby." "Entrepreneurs are weird people... they will try to protect it."
- "with entrepreneurs, they will be keeping that with their clothes [close], and they will not want to give it back."
- "that's exactly the reason why they came to us in the first place. They're struggling with letting things go, they're struggling with delegation."
- "a lot of that is the result of them being burned before by somebody else who didn't deliver."
- SOPs live in founders' heads: "hey, I know that when somebody messaged me on WhatsApp, I have this template that I will send them, and then I will notify in CRM. They remember that in their head."
- "The problem with most founders is that their context lives in their head, which makes them the bottleneck."
- Second brain is "like, a number one requested thing by entrepreneurs."
- AI slop frustration: "whenever I see somebody opening ChatGPT and saying, like, write me an email, and that's their whole thing, that frustrates me." Goal: "feels like Jarvis... not just AI slop."
- Founder-facing objection handling (generalizable): "Now this is a trade. So they sacrifice their... disbelief or lack of trust in order to get the result that you're promising."

## Jargon & Pareto terms
- **Right Hand**: Pareto's placed executive assistant (Ivan: don't be a VA, "become something different, something bigger").
- **Second Brain**: full knowledge system of linked markdown files + connectors; "not just drag and drop a couple of files."
- **Context layer / Action layer**: static knowledge folder / live connectors.
- **MOC**: Map of Content, per-folder index.
- **Frontmatter**: YAML metadata header. **Wikilinks**: double-bracket links between notes.
- **CLAUDE.md**: root instructions file for Claude in the brain.
- **Reverse interview**: AI (or Right Hand) asks the founder structured questions to build the brain.
- **Librarian, not shelver**: humans feed and oversee; Claude files.
- **Daily extract**: daily routine pulling promises/decisions/tasks with sources.
- **Morning Brief**: daily deliverable (commitments, blockers, ranked ship list, meeting context).
- **Retrieval test**: verify brain finds the right file.
- **Handover document**: session summary saved to the brain for the next session.
- **Routines**: Claude scheduled tasks. **Artifacts**: Claude-built pages/apps as deliverables.
- **MCP**: Model Context Protocol. **EOR**: employer of record.
- **Second Brain Workshop**: Pareto's paid founder training ($100/seat) and done-for-you build ($500).
- **Plaud / Omi**: AI wearable recorders feeding the brain.

## ICP / personas / offer signals
- ICP (verbatim): US SMBs, "Primarily founder-led companies. Usually making at least $500,000 a year." Sales cycle ~2 weeks.
- Persona traits: protective of their business ("their baby"), struggle with delegation, burned before by people who didn't deliver, context trapped in their head, ~14 systems in their head.
- Offer mechanics: monthly retainer; Pareto as EOR and trust "guarantor"; weekly 90-min Friday founder delegation training; Right Hands trained in AI (second brain, morning brief, connectors) as differentiator vs VAs.
- Second Brain itself is a monetized founder offer (workshop $100/seat; build-out $500) and a strong lead-magnet candidate (number one request from entrepreneurs; 14 systems -> 1).
- Pricing for the Right Hand retainer: not stated on Day 3.
- Guarantees: none stated beyond Pareto vouching for its people.

## Brand / tone signals
- Slide deck voice: short declarative headlines ("Context is what rules now", "Access is earned, not assumed", "You are the librarian, never the shelver"), "THINK OF IT LIKE" analogies, numbered blocks. Slide colors/fonts not visible in text export.
- Ivan's voice: blunt, direct, anti-fluff ("No affirmations", "AI slop", "no emotional cushioning"), big-picture hype ("trillion dollar nuclear supercomputer that costs you $20").

## Competitors / alternatives mentioned
- Generic VAs ("will be replaced at mass... by AI"); ChatGPT used shallowly; Codex (ChatGPT) as alternative to Claude Code; "Obsidian second brain" framing dismissed.

## Lead magnet / funnel hints
- No explicit lead magnet taught. Relevant assets: Second Brain Workshop prompt (company + entrepreneur-as-person versions), the 14-systems stat, the reverse-interview questionnaire (identity, offer, team, people, tools, sensitive data, jargon, "what lives in your head"), the Morning Brief format, the six-ways-it-breaks list, the retrieval test.
- Using transaction data for marketing: analyze LTV (average vs median) and most popular products, "craft a message that will be relevant to people who actually pay you money."

## Homework (slide, exact)
"Build a starter Second Brain for your sample founder: Kasim Aslam.
- Ask Claude to design the folder architecture and generate it as a downloadable zip. Download it, unzip it, and drag the whole structure into Google Drive.
- Run an intake from mined material (Extracted from transcripts, documents, scraping, etc.)
- Populate the context layer with at least five documents: at least one document covering identity, offer or pricing; at least one document covering team or key people; at least one longer-form piece: a transcript, a podcast, a written history.
- Upload those same markdown files into a Claude Project. (This is your free-plan replacement of a live Drive connection)
- Run the retrieval test and record it: three questions you already know the answers to; show it finding the right file, not just producing a plausible answer.
- Prepare a quick tutorial for your founder showing how it works.
Submit to: bootcamp.paretotalent.com/homework. Remember to: Post your homework in #Homework. · Share one thing you liked a[bout…]" (slide text truncated in export)
- Live version (transcript) differed: set up Drive folder, let Claude design architecture, run intake, 5+ docs, connect at least one action-layer connector, retrieval test; Ivan said he'd verify feasibility and post the revised homework in the homework tab. The slide version above appears to be the revised one (zip + Claude Project as free-plan workaround).

## Final project hints
- Pareto has an SOP for final projects: announced on the last day of the bootcamp, delivered as written instructions via Slack, with agenda, requirements, scoring rubrics and score definitions.
- Sample founder throughout is **Kasim Aslam**; second brain is meant to be reused later ("whenever you will be building a landing page for, let's say, Kasim. You won't need to repeat yourself").
