---
type: source
source_type: transcript
title: Pareto Bootcamp Day 4
captured: 2026-10-03
origin_url: https://drive.google.com/file/d/1gJjSHiuNaUfZBkdGLJgH4Ptdl_mWKrfb/view?usp=drivesdk
slides_url: https://docs.google.com/presentation/d/1pIQCL0KkxSN_66tJrzunyG9-tbBuFA-E0xeEfn7_KQk/edit?usp=drivesdk
speakers: [Ivan Bunin, Amparo Linares, Franco Mancebo, Jade Gonzalez, Gorro Rieznik Aguiar, Julián Soerensen, Isabel Darsin, Chiara Aymonino Sicco, Alex Viciano, Valentin, Diego Garin, Francisco Guillamondegui, Juan Nonis]
tags: [bootcamp, day-4, claude-skills, slash-commands, mcp, subagents, routines, automation, zapier, n8n, gohighlevel, shortwave, linkedin, kasim-voice, right-hand]
status: draft
---

# Pareto Bootcamp Day 4: Claude Skills, Subagents & Automation

Related: [[company-overview|Pareto Talent]] · [[right-hand-program|Right Hand Program]] · [[ivan-bunin|Ivan Bunin]] · [[kasim-aslam|Kasim Aslam]] · [[bootcamp-day-3]] · [[bootcamp-day-5]]

Sources: slide deck "Pareto_Bootcamp_Day4" plus the full transcript "Pareto_Bootcamp_Day4 - Transcript.txt" (about 2h05m; read in full). Both are titled Day 4.

## Topic of the day
The slide framing is "You have context. Now give it hands." Day 2 taught the model what it needs to know. Day 3 gave it somewhere to keep that knowledge (the second brain). Day 4 is where it "stops answering and starts doing." Ivan: "we just have a, like, smart brain, but brain without being able to execute is pretty much useless."

Most of the session was one live build. Ivan made a **LinkedIn post skill in Kasim's voice**, connected Canva to it to produce graphics, scheduled the result through GoHighLevel's social planner, and then turned the whole thing into a daily **Routine**.

## Session outline (slides: "Today's Plan")
1. Skills: one capability, one file
2. Slash commands: how you actually fire one
3. MCP: plugging Claude into Drive, Gmail, Slack, Notion
4. Subagent vs Agent Team vs Workflow
5. Real examples, and where Zapier and n8n fit

How the class actually ran:
- Intro. Ivan said online courses are already outdated: "if you go to, again, Udemy and buy a course, it's already outdated", and Zapier course authors won't update for AI "because otherwise they're shooting themselves in the leg."
- Skills concept, then gathering context for the LinkedIn skill: scraping posts, YouTube transcripts, Kasim podcasts and Delegation Mastermind transcripts.
- Visual templates: a "holding a card" mockup made in ChatGPT and a Twitter-style Canva template. Canva was connected as a connector.
- Skill → Input → Output → Post pipeline design, then the automation building blocks (trigger, condition, action, wait).
- Q&A (context window vs limits, second brain vs context, wait steps).
- Skill finished, then scheduled through the GoHighLevel private integration (API key kept in Apple Passwords/keychain), then webhooks, then building MCPs for tools that have no connector.
- Routines, real example ideas, Zapier/n8n (Pareto's own Zaps), pitfalls, the Shortwave inbox tool, homework, Q&A and close.

## Frameworks and models taught

### 1. Skill (the unit of reuse)
- Definition (slide): "One capability, one file." Analogy: Claude is "a professional chef, dropped into an almost-empty kitchen." A Skill is "a recipe card you write once and tape to the fridge: one dish, done exactly the way you like it, every single time you ask for it."
- Ivan's version: a repetitive task, which "could be a mix of prompts with the context, with best practices, with the checklist." Skills "systematize the delivery and ensure that each time it delivers the result, it's within the constraints of the SOP that you provided."
- Claude sometimes creates skills for itself when it sees repeated requests. Skills are logged so Claude knows they exist ("logged within ClotMD file", i.e. CLAUDE.md) and can be triggered automatically when relevant.
- **Inside a SKILL.md (4 parts):**
  1. Name & description: what it does and when to reach for it ("the line Claude reads to decide if this Skill fits the moment").
  2. Tools: exactly which tools it may touch. "Narrow this deliberately, every time."
  3. The instructions: plain English, steps in order, "the way you'd explain it to a new hire."
  4. The standard: "What counts as done well, not just done."
- In most cases you don't write these fields by hand. You build the skill in a session with AI and it fills them in. Skills "should be rooted in context," meaning your SOPs and actual materials.
- **Works vs doesn't work:**
  - Doesn't: "Help with content." (too broad); twelve steps covering three unrelated jobs; no standard; assumes context not written in the file.
  - Works: "Draft a LinkedIn post from a call transcript." (one job); five steps serving one outcome; "A stated quality bar you could argue with"; everything needed is an input or written down.
- Skill folder structure (shown on the built skill): the folder is the skill, and a `references/` subfolder holds Kasim's voice, visuals, post structure, platform behaviour and frameworks.

### 2. Slash commands
- "A slash command is you calling out the dish by name" (analogy: "Hey Siri, good morning").
- Three steps: You type it (`/standup`) → Claude reads the Skill → "Same shape, every time" (Yesterday / Today / Blockers).

### 3. Context gathering for a voice/content skill (live method)
Context Ivan listed for a LinkedIn skill:
- Previous posts (your own)
- Voice: anything that teaches "how we speak"
- Best posts from creators who "do well with my audience", e.g. Codie Sanchez ("She speaks to a lot of entrepreneurs, so she speaks to my people, to my ICP") and Dan Martell
- Best practices (copywriting, hooks, CTAs, platform algorithm), e.g. YouTube transcripts, taken "with a grain of salt"
- "The meat": pillar content, calls, books, podcasts. "places where we actually said things that we want to transmit in the universe." Rooting the skill in your own words means it "will not be sounding as a slop anymore."
- Proprietary data: Delegation Mastermind transcripts, Kasim's hiring book
- Creatives/visual templates
- Balance: too little material leaves it "underwhelmed" and 100 books leaves it "overwhelmed". "it's our job to define what are the resources that I want to lock it in." Expect to experiment.
- Watch out: AI-generated posts can quote private client conversations if messages and emails are connected. Ivan showed a post that "quoted a particular client what he said to me on a call."

### 4. Skill → Input → Output → Post (automation design)
- Skill (writes content) → Input (the meat; "needs to be coming in all the time," e.g. calls and Instagram videos, or you run out of topics) → Output (Canva image + post copy = "fully assembled post") → Schedule/post to LinkedIn.
- "start with a whiteboard, or start with a piece of paper, to map it out." If you jump straight into building, you end up "the human barrier that prevents AI from being able to run all of this."
- "What I want you to extract from all of that is the concepts."

### 5. Automation building blocks: Trigger, Condition, Action, Delay/Wait
- Slide: "every automation you'll ever touch is built from these four pieces."
  - **Trigger:** "The event that starts everything: a new email lands, a form gets submitted, a deal changes stage."
  - **Condition:** "A check before anything fires: only continue if the sender is a real client, not a newsletter."
  - **Action:** "The thing that actually happens once the trigger and condition both pass."
  - **Delay:** "Optional pause... wait one full day before the follow-up fires."
- Life analogy: rain (trigger), it's wet and I need to go out (condition), take umbrella (action).
- LinkedIn example built with students: trigger is a schedule (daily 9 AM) or a meeting/form as new input. Condition is guardrails/confidentiality (stop if the post holds a name, an amount of money, a password, or anything offensive). Action is schedule the post. Wait is post every evening (a better time).
- Applies to "Zapier, NA10 [n8n], GoHighLevel, routine inside of the cloud". All of them follow the same pattern "because that's basically how we behave as people."

### 6. Webhooks vs API
- "An API is the phone line. A webhook is the phone actually ringing." A webhook is "an instant notification fired the second an event occurs."
- Ivan's GHL example: push a webhook (POST request with custom data such as full name) from a GHL workflow to Claude, which uses it as a trigger.

### 7. MCP (Model Context Protocol)
- Analogy: Claude is a brilliant assistant in a small walled-off office. "An MCP is a new ability plugged straight into that office." Model = Claude, Context = what Claude can see or touch, Protocol = "the standard plug."
- Old way (manual Zapier: connect Gmail, filter, route to Slack, test, debug, repeat for every automation) vs new way (plain English, e.g. "alert me in Slack when I get an email from Kasim." Claude connects Gmail and Slack through MCP, builds and tests it, and you review).
- Connections worth having: Google Drive, Gmail, Slack, Notion, Calendar, a CRM.
- If no connector exists (e.g. GoHighLevel), google "<tool> MCP", paste the guide link into a new session and ask AI to connect it. "AI uses you as a… human version of itself."
- **"Connections are permissions" (the rule that never bends):** treat a connection "exactly like handing over a password"; "Scope down, never up"; never let a connected tool touch credentials files, raw passwords or API keys; on client work "ask before you connect anything new. Every time." "This is the fastest way to lose a founder's trust."
- API key hygiene: store tokens in Apple Passwords/keychain, Bitwarden or 1Password and point AI to them. Pasting into chat is a "bad practice" ("sometimes I do that"). Rotate keys you have exposed.

### 8. Subagent vs Agent Team vs Workflow (slide)
All three live in Claude Code, so Pro is the floor.
- **Subagent** (Pro): can fire automatically, or you trigger it ("bring in a research subagent and find everywhere we've mentioned pricing"). No extra cost.
- **Agent Team** (Pro, token-heavy): always manual. One-time setup (flip an environment variable, restart Claude Code). Prompt: "use a team, split this across 3 agents." Burns 2 to 4 times the tokens of a Subagent.
- **Workflow** (Max required): always manual. Say the keyword first: "ultracode migrate this app and fix every test."
- (Not covered in depth live.)

### 9. Routines (the layer that starts itself)
- "A Routine is a prompt or a Skill with a schedule attached instead of a person attached." Hourly, daily or weekly. Analogy: "the specialist who already knows to show up every morning at 7."
- Create one by asking: "Can you prepare a routine that will run every morning at 9 A.M. for me?" Edit one by starting a new session with the routine's name. Routines show in the left sidebar with active state, frequency and run history.
- Limitation: Claude runs locally, so "you need your computer to be active when the task is scheduled." Zapier and n8n run in the cloud 24/7.

### 10. Zapier / n8n: where they fit
- Zapier: "fastest way to wire two apps together when the logic is simple and linear." n8n: "more technical and far more customisable," self-hostable.
- "Neither one thinks. They move data on rails you already built. Claude is what decides and writes."
- "Zapier/Make/N8N as the nervous system that never sleeps, Claude as the judgment for the one step that actually needs thinking."
- A HighLevel deal changing stage at 2 AM "needs something watching at 2 AM." Zero-judgment data moves shouldn't pay for model reasoning.
- ROI rule: a 5-minute automation replacing a 2-minute manual task pays back after 3 runs. "This is like an investment."

### 11. Common automation pitfalls (5)
1. No error handling: "it breaks silently and the client finds it first."
2. No idempotency: "Run it twice by accident and it sends the email twice."
3. No human checkpoint: "Anything that talks to a client or moves money gets a person in the loop, always." Ivan: "if something will post that you were not supposed to post, guess who will be liable?... you will not be able just to come to your employer and tell, hey, you know what, Claud screwed up."
4. Scope creep on tools: "A Skill given broad access 'just in case' is a Skill nobody fully trusts."
5. No test run: "Never let the first real execution against a client's data be the first execution at all."

### 12. Human checkpoint in inbox work (Shortwave pattern)
1. Draft, don't send: a sensitive reply goes into a To-Do with the draft attached, and the founder clicks send.
2. Leave a note on any email: a comment on the thread for whoever picks it up.
3. Label once, it remembers ("do this going forward").

### 13. Red-teaming a skill (Q&A)
You can't guarantee you covered everything. Ask AI a "contrarian statement": "analyze everything that can go wrong with this skill," then implement the fixes. Each time it fails, tell it and have it patch the skill. "AI will make mistakes... it's unreasonable for us to expect it not to."

### 14. The 80% rule
"we are going for 80%. We need something to be 80% good. Once it's 80% good, ship it... Don't wait until it's perfect." Ivan credits this to Kasim ("something that Casim is great at").

## Numbers, stats, proof points
- Live LinkedIn analysis (about 100 scraped posts from Dan Martell + Codie Sanchez; 50 per creator scraped with Easy Scraper):
  - Hooks under 40 characters perform better ("hook length is the clearest signal").
  - Posts with links get about half the engagement. Dan Martell's median is about 460 with a link vs about 913 without (transcript: "460 median with a link, it's, 463 without 913").
  - Martell posts "naked text" (no image) 7 times out of 56, and those perform worse. Takeaway: never post naked text.
- YouTube transcript pull: about 600,000 characters of context; 22 videos scraped from one search results page.
- Delegation Mastermind: Pareto's closed weekly session for Pareto Talent clients, **every week for 90 minutes**. Proprietary content that isn't public.
- Pareto has a hiring book ("the higher book... the book on hiring"), gated behind a form.
- Building the whole LinkedIn system took about 60-90 minutes live: "in 90 minutes, we were able to build somebody a full social media content plan and presence."
- Lead dossier: saves "20, 30 minutes" of research per meeting (slide: "Saves the ten minutes everyone skips under pressure").
- Onboarding automation: about 10 minutes per person by hand. "Imagine onboarding 100 people."
- GoHighLevel costs $97 ("It's 97, but it can replace all of this software").
- Ivan spends "6 hours out of my 8 hours a day in Cloud [Claude]."
- Bootcamp: day 4 of 10 ("We have 6 more days"). Ivan says those still keeping up are "already probably the top 5% of everyone." The first 3 days were deliberately complex "to boil down everyone who's not able to keep up."
- Agent Team uses 2 to 4 times the tokens of a Subagent.
- Context window: compacting is offered at about 70-80%. A student reported a 1M-token context, half used after 3 days.
- Claude Projects "can hold, up to 100 pieces of context."

## Stories (2-4 lines each)
- **AI quoted a client:** Ivan showed a Pareto social post that AI had built from connected messages. "It actually went ahead and quoted a particular client what he said to me on a call." Lesson: connecting emails and messages can publish things you didn't want public.
- **Kasim "holding a card" mockup:** Ivan used ChatGPT to make an image of Kasim ("a tall dude in a black t-shirt") holding a blank white board, from Pareto Talent photos. He cropped himself out with Photopea so the AI wouldn't use his face. Proving the concept with AI comes first, and paying a photographer comes only if it works.
- **First skill output (sample post):** hooks like "research is procrastination for you. It's weaponization for your right hand." / "I didn't save time, I built a person who runs it better than I do." / "most founders delegate the task and keep the research. That's backwards." It mentioned a septic business run by "Agustina." Canva graphic text: "You don't have a pipeline problem, you have a bottleneck named you."
- **GHL token expired live:** scheduling failed, so Ivan created a new private integration ("Ivan Claude") with social-media scopes, saved it to Apple Passwords and pointed Claude to it. Then he rotated the key because students had seen it. The post was then scheduled for Sept 26, 9 AM in the GHL social planner.
- **Bootcamp application automation (wait step):** step 1 survey submitted (trigger), then condition: phone country code inside LATAM ("we are currently not accepting outside of LATAM"). Then a 2-hour wait for step 2. If step 2 isn't submitted, an email goes out ("hey, you're almost done, finish it"), and it waits and loops.
- **Webhook joke example:** if someone abandons the bootcamp application, a GHL webhook could trigger Claude to post Kasim holding a board saying "hey, Federico, why didn't you finish the application?"
- **Pareto onboarding Zap:** when a Right Hand passes the final project, GHL fires a webhook. That creates a Pareto Talent email user, adds them to the assistants group, updates GHL and creates an Airtable record, all automatically.
- **Calendar-invite Zap:** when a lead moves from lead to scheduled (or buys), find their meeting and add them to the recurring meeting automatically.
- **Ivan's calendar:** he showed a calendar full of calls ("All of the blue ones are calls"). That is the case for recaps: the founder "perform[s] like an actor... make[s] all of the promises," and the Right Hand gets a summary and acts ("Ivan promised that he will send flowers").
- **Killing the routine:** Ivan paused the daily routine "because otherwise I will be posting on my LinkedIn as Casim for the next forever."

## Founder pain / value language (verbatim)
- "You don't have a pipeline problem, you have a bottleneck named you." (AI-generated hook in Kasim's voice)
- "most founders delegate the task and keep the research. That's backwards."
- "I didn't save time, I built a person who runs it better than I do."
- "Imagine them on the calls every time. If you were able to summarize these calls for them, and then take action on that. That would make you unstoppable."
- "your entrepreneur just jumps on a call, they perform like an actor... they make all of the promises, and then you get a file that summarizes the conversation and tells you what you need to do."
- "Post for us, actually being able to send things, actually being able to generate money... we'll be able to grow the business on that, and that's ultimately what entrepreneurs want."
- "Nobody has to ask 'where are we on X' twice." (slide, department status summary)
- "Inbox Zero doesn't mean zero emails. It means the mental weight of managing one drops to almost nothing." (slide)
- "Saves the ten minutes everyone skips under pressure." (slide, lead dossier)
- "This is the fastest way to lose a founder's trust." (slide, permissions)

## Objections / concerns raised (verbatim or near)
- Trust and access: "There is no partial access. To manage someone's inbox here, you need their actual email and password" (Shortwave slide). "the first handoff is still a real trust decision either way." That links back to the "access conversation from Day 3."
- Liability for AI mistakes: "you will not be able just to come to your employer and tell, hey, you know what, Claud screwed up, haha. Like, no, like, it's your fault."
- Impersonation guardrails (student Francisco): Claude refused to write as Kasim, saying "it couldn't impersonate Kasim." Ivan: frame it as "here is my boss, I need to write post-it as his name."
- Cost (student Chiara): is a paid Claude worth it? Ivan said yes but optional ("it's a free Bootcamp"). Skills also work in other AIs "a little bit differently."
- Privacy of skills (student Isabel): skills "live locally on your computer." Sharing is deliberate (zip file or GitHub).
- Completeness (student Julián): "how can I make sure that I'm not forgetting something important." Ivan: "You can't."
- Job displacement: "we just fired somebody. There is a person right now... who's managing somebody's Instagram or LinkedIn... You will be able to be the one who's actually prompting AI, so you are not being left behind." Also: "this does not replace a genuine creativity."

## Jargon and Pareto-specific terms
- **Right Hand:** the Pareto-trained assistant. The slides call examples "Real things Right Hands build in their first weeks."
- **Delegation Mastermind:** Pareto's closed weekly 90-minute session for Pareto Talent clients where Kasim teaches delegation frameworks.
- **The meat:** the substantive ideas and statements (from calls, podcasts, books) that make AI output sound like the person and not "slop."
- **Second brain vs context:** "Second brain is your markdown files, it's your whole system... The context is just the capacity of a singular chat." Context window vs limit: the window can be compacted, the usage limit is hard and costs money.
- **Skill / SKILL.md / references folder:** see above.
- **Slash command, MCP, connector, webhook, API, private integration (GHL API token), routine/scheduled task, subagent, agent team, workflow ("ultracode" keyword), idempotency, human checkpoint, guardrails.**
- **Lead dossier, department status summary, meeting-to-recap, daily morning brief:** standard first-week Right Hand builds.
- **GHL / GoHighLevel / High Level:** CRM Pareto uses (social planner, workflows, private integrations, webhooks).
- **Easy Scraper:** Chrome extension used to scrape LinkedIn posts and YouTube search results to CSV. **Apify:** for scaling scraping. **docs.new:** shortcut to create a Google Doc. **Photopea:** online Photoshop.
- **CSV:** "Excel, but without a table, with just commas"; easier for AI to digest than Excel.
- **Inbox Zero:** the reduced mental weight of managing email.

## Tools named
Claude / Claude Code (Pro, Max, Teams), Claude Projects, ChatGPT (Ivan uses it "primarily for image generation"), Canva (connector, templates), GoHighLevel ($97; social planner, workflows), Buffer (LinkedIn scheduler with API), Zapier, n8n, Make, Airtable, Fathom, Gmail, Slack, Notion, Google Drive, Calendar, Telegram, Apple Passwords/Keychain, Bitwarden, 1Password, GitHub (shared skills), Loom, Shortwave (Ivan has also tested "all of the superhumans"), Easy Scraper, Apify, Photopea.

## Shortwave (Pareto's preferred inbox tool)
- "the best email management tool from all of the ones that I tested... That's the tool that we are using here in Pareto Talent... and that's the tool that a lot of our assistants are using as well."
- AI-native client on top of Gmail with a built-in AI assistant, To-Dos instead of a flat inbox, Snippets (reply templates), and comments/assignments.
- Three upgrades: To-Dos group every email tied to a task; "It knows your voice" ("tell me about Sam, draft a reply"); "It catches what you dropped" (scan the last 3 weeks against the calendar for un-followed-up calls, plus Snooze).
- Trade-offs: Gmail only (no Outlook or Yahoo), needs the actual email and password, logs in per device.

## Real first-week builds (slides: "Top things worth building your first week")
1. **Lead dossiers:** name + company in, public context out, structured against a fixed template, "a one-page brief before the call starts." Live version: triggered when someone books, it checks LinkedIn and Gmail history and sends a PDF to email or Telegram.
2. **Department status summary:** pulls Slack, calls, emails and CRM for one department and posts one daily status update.
3. **Meeting-to-recap:** pulls the Fathom transcript, drafts a follow-up in the founder's voice, and leaves it as a draft until a person sends it. "the safest kind of write access to hand someone in week one."
4. **Daily morning brief:** connects Gmail, Fathom, Slack and Calendar, flags what needs a decision, checks the week ahead, and gives a "short summary the founder can read in two minutes on Sunday night." Ivan is building his own as a dashboard.
- Also mentioned as routines: daily posting, daily inbox analysis, daily competitor research, removing junk emails and cold pitches.
- Multi-tool sequencing example for inbox: Gmail → Fathom (did we have a call?) → Slack (ping Ampi) → output.

## ICP / persona / offer / brand signals
- The Right Hand serves "entrepreneurs" and "founders" who are on calls all day and make promises. A founder's real credentials and inbox access is a trust decision.
- Content ICP: Ivan chose creators who "speak to a lot of entrepreneurs" (Codie Sanchez, Dan Martell) as matching "my ICP."
- Kasim: "very tall"; speaks on the Genius Network ("That's insane"); has podcasts; teaches delegation frameworks in the Mastermind. Ivan calls him "my business partner." In the Canva template his "handwriting" font should "look bad." Visual formats for Kasim posts: holding-a-card board and Twitter/tweet mockup.
- Bootcamp: free ("it's a free Bootcamp"), LATAM-only applications (phone code check), a multi-step application with personality tests ("done all of these personality tests"). Passing the final project triggers onboarding as a Pareto assistant with a Pareto Talent email.
- Pareto uses: GoHighLevel (CRM, social planner, bootcamp workflows), Zapier (calendar invite, invoice forwarding, applicant intake, onboarding, "predictive index complete"), Airtable, Shortwave, Fathom, Slack.
- Pareto's hiring book is gated behind a form (a lead-magnet example).
- No pricing, guarantee, brand color or font specifics for the Right Hand Program were given on Day 4.

## Competitors / lead magnet / funnel hints
- The bootcamp application flow is itself a funnel example: survey step 1, LATAM filter, 2-hour wait, "you're almost done" email reminder loops.
- LinkedIn content findings for any funnel content: short hooks (<40 characters), no links in the post, always include a visual (card or tweet mockup), CTA at the bottom, avoid "trigger words that demote your posts."
- Gated hiring book = existing Pareto lead magnet.
- Shared skills on GitHub (people have shared "a bazillion of skills").

## Homework (Day 4, exact from slide)
"Build a real Claude Skill for one task, and connect it to a real tool."
- "Pick one task you would genuinely do more than once. Narrow beats impressive."
- "Create the SKILL.md for the tasks together with Claude: A name and a description that would actually make it fire correctly. The inputs, the steps, the quality standard, and the exact output shape."
- "Test it with its slash command. Run it at least twice with different inputs."
- "Connect at least one MCP so Claude can act on a real tool, not just talk about it."
- "Share your skill with the group in the homework session and record a quick Loom explaining what this actually does."
- Submit to: bootcamp.paretotalent.com/homework. Post in #Homework; share one thing you liked in #General.
- "Upload the finished SKILL.md on: Settings → Capabilities → enable Code execution, then Customize → Skills → upload the file."
- Clarifications: any skill is fine ("up to you"). Share it as a zip, no GitHub needed. Connect your second brain so the skill reuses existing context ("we are just fixing all of this research once and for all"). Homework can be resubmitted.

## Final project hints
- Homework is checked during final project review: "you didn't do good enough on the final project for the landing page, but your homework on the landing page was cool." The final project includes a landing page.
- Passing the final project triggers acceptance and onboarding automation.
- Upcoming days: Day 5 is GoHighLevel ("one of the most fundamental softwares"). Later days cover landing pages, apps, automations, email marketing, content/video editing, image creation, inbox management, calendar management and personal productivity. Teaching style: "strategies and tactics," not click-by-click.
