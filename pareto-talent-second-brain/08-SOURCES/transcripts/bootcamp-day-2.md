---
type: source
source_type: transcript
title: Pareto Bootcamp Day 2
captured: 2026-10-03
origin_url: https://drive.google.com/file/d/15db3QkZhziiqhK30oZOuBPwIj1eSxMon/view?usp=drivesdk
slides_url: https://docs.google.com/presentation/d/19iQx8FVyeA1nh3IRt73S6fvtaYiDO02JlvIR-PEzMqA/edit
speakers: [Ivan Bunin, Amparo Linares, Mrika Berisha, Maria Muñoz, Demian Nazareno Ducardt, mario meneses, Agustina Rojas]
tags: [bootcamp, day-2, ai-fundamentals, context-engineering, prompt-engineering, claude, projects, agents, markdown, kasim-voice, second-brain]
status: draft
---

# Pareto Bootcamp Day 2: AI Fundamentals, Prompt Engineering & Agents

> Distilled source note. Not the raw transcript. Facilitator: [[ivan-bunin|Ivan Bunin]] (co-founder). Deck built by Amparo Linares ("Ampi"), Ivan's executive assistant. Both source files are titled "Pareto_Bootcamp_Day2", so the day number is confirmed.

## Topic of the day

The slides frame it as **"Yesterday was the job. Today is the craft."** Day 1 was what Pareto expects from a Right Hand, and from Day 2 the trainees are building. The core thesis, in the deck's words:

> **"Context is king. Prompt is second."**
> "A mediocre prompt with the right context beats a beautiful prompt with none."
> "Your job is not to write clever instructions. It is to assemble what the model needs to know before it starts."

Ivan put it this way: "The prompt is not the problem, the context is the problem." He also said "Prompt can be simple, the context needs to be extended."

## Session outline (slides + transcript)

1. Welcome and homework check. Ivan says he deliberately tries to "scare as many people off as we can": cohorts shrink every day so that "the best of the best" are left at the end.
2. Why AI on Day 2: "if you are not using AI ... from that professional standpoint, you're already at that weight in the company." At first the bootcamp covered AI only briefly. "Right now, it's the core of the work."
3. AI 101: four kinds of AI; how an LLM predicts the next word.
4. Why the bootcamp standardizes on Claude.
5. Context vs. prompting: the "random number 17" exercise and the evolution of prompt engineering.
6. Context engineering steps: Gather, Clean, Load, Ask.
7. Six context sources, with live demos: Fathom calls, YouTube, Google Drive, websites/scraping (FireCrawl), dictation (WisprFlow), email threads.
8. Markdown as the universal AI language, plus processing transcripts into markdown "knowledge material".
9. Projects: their anatomy and five instruction lines. Live build of a "Kasim voice" Facebook-post Project.
10. Advanced context mining on Kasim: Easy Scraper (Facebook/LinkedIn), Google `filetype:pdf` search for his books, Claude Code + Apify to download, transcribe and summarize his last 50 Instagram reels.
11. Agentic workflows: Chat, Project, Cowork, Code; when to use chat vs. agent.
12. Safety and data privacy: what never to paste.
13. Tool landscape, tomorrow's stack (Day 3 = Second Brain), homework, Q&A.

## Frameworks and models taught

### Four kinds of AI (slide "AI 101")
- **Supervised learning**: "Learns from labeled examples, mapping known inputs to known outputs." Examples: spam filters, fraud detection. Ivan called it "basically a huge conditional logic".
- **Unsupervised learning**: "Finds patterns and groupings in data nobody labeled first." Examples: customer segmentation, anomaly detection.
- **Reinforcement learning**: "Learns by trial and error, rewarded for good outcomes over time." Examples: self-driving cars, game-playing AI.
- **Generative AI**: "Creates new content instead of just classifying or predicting it." Text, images, audio, video. "This bootcamp lives here."
- Ivan's point: agentic AI now combines these. It may write itself a Python script, the supervised style, or run tests, the reinforcement style. "For some of them, you need trial and error, for some of them, you need parameters, but for majority of them, for generative AI, you need context."

### What an LLM is
- "A model trained on enormous amounts of text to predict what comes next. It is not looking anything up and it does not know your business."
- The slide's analogy: "A brilliant new hire with no access to your files, your inbox or your history. Sharp, fast, and completely uninformed until you brief them."
- Next-word example on the slide: "My favourite food is a ... bagel ... with ... cream ... cheese."

### Weak input, weak output ("trash in, trash out")
Slide bullets:
- "The model cannot ask you for the file you forgot to attach."
- "It will not tell you it is guessing. It will guess confidently, in full sentences."
- "Vague in, generic out. Every time, with no exceptions."
- "When the answer is bad, ask what it did not know before you ask how you phrased it."

Ivan noted that "trash in, trash out" was true before AI too: "AI just amplified that."

### Two truths about AI (whiteboard segment)
- **Truth 1:** Without context, the AI falls back on the generic "best practice" from the internet. Ivan's demo: "Give me a random number between 1 and 25" returns 17 for most people. Asking for a "professionally sounding email" returns "the most generic email that doesn't mean anything." Ivan: "If you will be using AI without any context. You are doomed for failure."
- **Truth 2:** Prompt engineering (role + goal + voice, for example "imagine that you are ... CTO ... your goal is to write a professional email ... your voice is a serious but friendly") narrows the search. It "still works" for simple outputs. To go further you need to understand that "AI learns on data." Everyone shares the same generic data, but "what makes your data unique is your context. That no one else has." That is also what "makes AI not sound like AI."

### Context engineering: Gather, Clean, Load, Ask (slide "The Shift")
1. **Gather**: "Pull real material from where it already lives ... Don't write summaries from memory, go get the source."
2. **Clean**: "Strip out the noise ... If a piece of information doesn't shift the output, it doesn't belong in there."
3. **Load**: "Put it into a Project so it persists ... a permanent reference."
4. **Ask**: "Now the prompt can be one line."

Ivan's mental model for step 1: imagine you are briefing a real co-worker. For a landing page they might need the "logo, description of the company, my biography, maybe an offer, maybe client testimonials ... a video."

### Six context sources "you will use daily"
The slide says: "Every one of these is free, already in their stack, and almost never used properly."
1. **Call recordings (Fathom)**: "The single richest source of how someone actually thinks, argues and talks when they are not performing." Ivan calls it "number one" and says to "record all of the calls."
2. **YouTube**: "Free, long-form, unedited, and in their own voice rather than a marketer's." Get the text from Description > Show transcript. Google Drive videos also have built-in transcripts.
3. **Google Drive**: "Docs, decks, SOPs and anything the business already wrote down. The fastest context you will ever get." Ivan's demo used Pareto's assistant contract.
4. **Websites & scraping**: "their public positioning, written carefully, in their own words." Tool: FireCrawl, which scrapes a full page to markdown. Ivan's demo used ParetoTalent.com.
5. **Dictation (WisprFlow)**: "Talk for two minutes instead of typing for twenty." This is also how you become the context source: "you are the context."
6. **Email threads**: "Real correspondence shows tone under pressure ... How they write when they are annoyed matters." Download the whole thread, not email by email.

Other context sources Ivan named: bootcamp transcripts and community posts, iMessage, Telegram, Instagram, SOPs, internal tutorials, and influential books.

### "Interview me" technique (dictation as context creation)
Prompt pattern: "I don't want you to use any of the knowledge that you have about this. I want you to interview me ... Ask questions one by one. And limit questions to 20." Ivan says Pareto's internal SOPs (scoring, application process, bootcamp process) were all built this way: "I just answered questions of AI about our process." The output (for example a one-pager) is exported as markdown and reused, "so I will not have to repeat myself ever again."

### Context mining: process before loading
"Instead of using raw transcripts, we are first processing these transcripts, we are first understanding what is the value, what is the knowledge material, what is the gold, and only then we populate it as a context." Prompt used: "extract all of the value pieces and then structure for me an output file that will be in Markdown format." Dumping raw CSVs and PDFs straight in "will do it poorly."

### Projects: persistent context (slides "The Fix" + "Anatomy")
- Definition: "A Project holds instructions and knowledge that apply to every conversation inside it."
- Analogy: "briefing a contractor on every single call, and hiring someone who already read the handbook."
- Ivan's definition: "project is a series of tasks that are together in one place." Instructions "tell AI how to do", knowledge tells it "what to do".
- **Anatomy**:
  1. **Instructions**: who it acts as, who it writes for, what it must never do. Written once.
  2. **Knowledge**: the source material. "This is the part almost everyone under-feeds, and it is the part that decides quality."
  3. **Examples**: "Two or three pieces of real output in the voice you want."
- **Three source types minimum**: (1) a transcript, for "how they speak when they are not writing"; (2) a document, for "how they write when they are being careful"; (3) a website or public page, for "how they position themselves to strangers". The slide adds: "One source is just imitation. Several give you a voice."

### Five instruction lines that do most of the work
1. **Who you are**: "You are the chief of staff to a founder who runs a 12-person agency." "Give it a seat, not a personality."
2. **Who you write for**: "You write for busy US founders who skim." "The reader shapes the output more than the writer does."
3. **How they sound**: "Short sentences. No hedging. Never uses corporate filler." "Describe the voice in rules, not adjectives."
4. **What you never do**: "Never invent a statistic. Never use em dashes. Never apologise." "Exclusions do more work than instructions."
5. **What done looks like**: "Output is ready to send with no editing." "Define the finish line or you will keep getting drafts."

### Agents and agentic workflows
- Slide definition: "An agent can take a goal, break it into steps, use real tools, check its own work and keep going until it is done." Analogy: "A chat tool answers your question. An agent goes and runs the errand."
- Ivan's definition: an agent is "AI that is actually in pursuit of achieving a goal," acting "on your behalf" through an "action layer".
- Three modes: **autonomous**, **scheduled** ("routine", for example every morning at 9 AM) and **trigger-based** (for example someone writes a comment). His example: check LinkedIn posts every Tuesday and analyze their performance. He says Claude now replaces tools like n8n and Zapier for him.

### Four ways to work with Claude (slide "Recap")
1. **Chat**: "One question, one answer. No memory across conversations." Good for "fast and disposable".
2. **Project**: persistent context. "You are still doing the work."
3. **Cowork (agentic)**: "Claude does the work ... uses real tools like Drive, Gmail and Slack ... Runs locally." Ivan: it asks for every permission and is "intermediary" between chat and code. The bootcamp mostly skips it.
4. **Code (agentic)**: "Reads and writes real files ... Steepest first hour, highest ceiling." Ivan: "least restricted," "no maximum" on files (chat caps uploads at 20).

### Chat vs. agent (decision rule)
- **Use chat when**: you want an answer, a draft or an explanation; the task is one step and you will review it immediately; you are exploring; speed matters more than completeness.
- **Use an agent when**: the task has dependent steps; it needs real tools (files, email, calendar, repo); you would otherwise repeat the same sequence weekly; the output needs checking against something.

### Markdown as the universal AI language
- Slide: headings, bullets and bold give a model structure it can follow. Claude, Obsidian, Notion and GitHub all read it. It is plain text, "never gets locked into one company's format."
- Ivan's file-format ladder: PDFs, Docs, images and MP4s are "harder for AI to read". TXT is easiest but "there is no structure at all". Markdown is "the easiest file for AI to read" because it is text with structure: `#` = H1, `##` = H2, `**` = bold, plus tables. It is "most similar to HTML" but without CSS or JS. Viewer: MarkEdit.
- Language rule: "use English for everything that you are doing within AI." Do not draft in Spanish and translate.

### Leverage and token-cost mindset
"If you are not able to break even on the tokens that you're spending on AI, then you're using AI wrong ... AI will pay for itself tenfold." Paying for tools rather than spending your own time is good leverage: "you're leveraging the most unleverageable resource ... your time." As a Right Hand, "these subscriptions, the Claud Pro, all of this is yours ... You will not be paying anything out of your pocket. That's the benefit of working for somebody versus just being a freelancer."

### Safety rules (slide "Before you touch real client data")
- "Never paste passwords, API keys, bank details or anything financial into a public AI tool."
- Training data carries the internet's biases.
- "The model will sometimes state a wrong fact with total confidence. Verify anything specific before it goes to a client."
- "If you would not paste it into a public Slack channel, do not paste it into a chat window either."
- "You are about to be trusted with a real founder's real business."
- Ivan: "the final quality control is you." You can opt out of training in privacy settings, but your data still passes through the provider's servers, so read the privacy policy.

## Numbers, stats and proof points

- **~2,000 calls** recorded at Pareto Talent over **~2 years** "with individual assistants, with our clients, with our leads, with all of the workshops." (Fathom, now on the paid plan.)
- **~6,000 documents** (markdown files) in Ivan's Obsidian second brain. "All of that makes my AI much better than your AI."
- Ivan processed **"more than 3 million words that I said"** to build an AI that sounds like him.
- **~95%** of the clients Ivan speaks with use Claude.
- Claude Pro costs **$20**. Ivan also has a Pareto team account plus a **$200** Max account.
- Typing benchmark: if you type below **140 wpm**, dictate. The fastest typers in the first bootcamp were about **90 wpm**.
- Ivan has **22 months** of WisprFlow Pro free through referrals. Pareto pays for WisprFlow for the whole internal team.
- Bootcamp facts Ivan dictated in the demo: free, **10 days, 2 hours a day**, live on Zoom, recordings provided, certification at the end. About **800 people live** planned. No fixed hire quota per cohort.
- VA cost comparison: having a Philippines VA download and transcribe 50 videos would cost "probably like 50 bucks, maybe more ... $1 per video". AI gives "$100 worth of output" for $1.
- Ivan: "it took probably a couple thousand hours, and I'm trying to compress it to you in 40."

## Stories (short)

- **Random number 17**: Ivan has everyone ask ChatGPT for a random number from 1 to 25 and most get 17. Without grounding, AI defaults to the internet's idea of "random". It is the opening proof that context beats prompting.
- **Nathan / BlueSense Digital Meta ads**: A generic "draft me a Meta campaign for a men's shoe company" prompt gives generic output. Adding the transcript of a 2-hour, 4-month-old tutorial by Nathan of BlueSense Digital grounds it ("UGC, founder iPhone videos"). Ivan had also met Nathan, and his own consulting call is "even better grounding truth". Adding the FireCrawl scrape of ParetoTalent.com means "AI knows what you sell, who to trust."
- **Amparo follow-up**: Ivan pastes a Fathom call with his EA Amparo, asks what she promised and what she is blocked on, then has the AI draft a Slack follow-up. The prompt was very short and the context did the work.
- **Bootcamp one-pager by dictation**: Ivan dictates the bootcamp offer and goals, then asks for a one-pager for his business partner. He exports it as markdown and reuses it as context.
- **Client testimonial to markdown**: Ivan turns a recorded client testimonial interview (with "Karen's entrepreneur") into a structured markdown knowledge file with key quotes.
- **Kasim voice Project**: Ivan builds a Claude Project for "Facebook posts" as Kasim's content manager. He loads YouTube/podcast transcripts ("10 months ago, hire top talent"), Easy Scraper CSVs of Kasim's Facebook and LinkedIn posts, a Google `"Kasim Aslam" filetype:pdf book` search, and Claude Code + Apify transcripts of Kasim's last 50 Instagram reels. One-line prompts then produce on-voice posts ("write a post about Kasim hiring Ivan").
- **Kasim's "safest way to school" robot story** (Ivan retelling "one of the favorite examples that Casim gives"): asked to get a child to school safely, the AI buys a Volvo and a car seat, "and then AI will go ahead and kill everyone around, because people are dangerous." The point is that AI pursues the goal by the most direct path and has no moral limits unless you set them.
- **Ivan's radical access**: his AI can reach his bank account, Pareto Talent's Stripe ("it can literally go ahead and refund all of the clients"), the CRM and his personal messages. He also runs Claude Code from Telegram on his phone at the gym. "So far, so good. Nothing happened. But I will keep you posted."
- **Data resale cautionary tale**: Ivan recalls (uncertainly) a middle-layer AI company that collected users' prompts and was "bought by Meta". The lesson is that AI companies "are hunting for the data".

## Pareto ICP, persona and offer signals (from this session)

- **Kasim's Facebook ideal reader**, as Ivan dictated it into the Project: "entrepreneur. Who's a founder of the company, Within, $500,000 to $5 million annual recurring revenue, or annual revenue overall, within United States."
- **Goal of Kasim's profile**: "Customs Profile should produce Pareto clients, And, peer network." Success in 90 days means consistently posting on his Facebook profile and getting more subscribers and engagement. Pareto is "not really active in Facebook groups as of right now."
- **Funnel shape**: Ivan's demo prompt was "top of the funnel post in Casim's voice, that will lead to a lead magnet in the end."
- **Slide example reader**: "busy US founders who skim". Example seat: "chief of staff to a founder who runs a 12-person agency."
- **Bootcamp's business purpose** (Ivan): (1) a philanthropic mission to train people; (2) "find top talent ... basically, it is a recruitment pipeline for Pareto Talent clients." Bootcamps are "application-only" and Ivan asks trainees not to share the recordings outside.
- **Right Hand perk**: AI subscriptions are paid by the employer or founder, unlike freelancing.
- Ivan's view of founders: "I see a lot of that in entrepreneurs, that they see the new shiny sink [thing], and they jump ship." His advice is "marry one tool".

## Kasim voice and brand markers extracted live (from the AI's analysis)

The AI's extraction from Kasim's content listed these recurring ideas and terms:
- "the Pareto rule"
- "our filtration process"
- proof story: "John Moran"
- "talking about miracles a lot"
- "Pay 10% above the high water mark"
- "fly traps"
- From the reels: "prepaid", "the graveyard", "borrowed pride" (the transcript also reads "Lukas prepaid", probably a mis-transcription)

Ivan's description of Kasim's writing: "short sentences, very, like, direct, so it actually conveys the point."

Kasim's content channels named: YouTube interviews, podcasts, Facebook profile, LinkedIn, Instagram reels, and books (PDFs findable online).

## Pain language and objections (verbatim, trainee and founder side)

- Ivan on founders: "they see the new shiny sink [thing], and they jump ship, and they try something different ... That is what will doom you to not actually getting any progress."
- On typing: "a lot of us, like, we hate typing. Typing is hard, typing is uncomfortable."
- On dictating context: "I know a lot of these things, but I don't have them written anywhere. I don't like writing."
- Implied objection about token cost: "if you are concerned about tokens and all of that ..." Ivan's rebuttal is the leverage argument above.
- Security objection: "if you're having concerns with the security, it's the right concerns."
- Trainee questions: Maria Muñoz asked "what are we actually creating with Casin's voice?" and Demian asked "if we can use OpenCon [OpenCode] instead of Cloud Code". Ivan answered "You can use any."

## Jargon and terms

- **Context / grounding truth**: the trusted material you tell the AI to treat as its source of truth instead of the internet.
- **Context engineering / context assembly**: gathering, cleaning and loading context. It replaces most of the work of prompt engineering.
- **Context mining**: extracting the "gold" from raw sources (transcripts, scrapes) into structured markdown before loading it.
- **AI slop** ("AI slope" in the transcript): generic, ungrounded output.
- **Second Brain**: an Obsidian vault of markdown files that feeds the AI (Day 3 topic). "Part of your role as executive assistant will be developing this second brains."
- **Project**: persistent instructions + knowledge (+ examples) for a recurring task.
- **Agent / agentic / action layer / routine / trigger**: see the frameworks above.
- **Right Hand**: Pareto's term for the executive assistant role (used in passing: "free training for right hands from Argentina").
- **SOP**: standard operating procedure ("how we do things").
- Tools: Fathom (fathom.video), WisprFlow (with a global dictionary of names and acronyms), FireCrawl, Easy Scraper (Chrome extension), Apify, MarkEdit, Obsidian, Claude Desktop/Code/Cowork, ChatGPT (Ivan uses it "only for images"), Gemini, Perplexity, Ideogram, Gamma, NotebookLM, Manus ("couldn't make it work really well"), Hermes (open-source self-hosted agent, "the most advanced"), n8n, Zapier.

## Competitors and lead magnet references

- No direct Pareto competitors were discussed. The only comparison was a Philippines VA charging about $1 per video for manual transcription, used to show AI leverage, not as positioning.
- Lead magnet: only the demo prompt "top of the funnel post ... that will lead to a lead magnet in the end." No specific magnet was named.
- External expert used as grounding: Nathan, BlueSense Digital (Meta ads).

## Homework (Day 2), exact from the slide

> **Build a AI Project trained on a real entrepreneur's voice.**
> Your target persona is Kasim Aslam.
> Source context from at least three different types:
> - A transcript, from a call recording, a podcast or a YouTube interview.
> - A document, from Drive or anywhere they have written something down.
> - A website or public page in their own positioning.
>
> Write the Project instructions covering:
> - Who it acts as, and who it writes for.
> - How they sound, described as rules rather than adjectives.
> - What it must never do.
>
> Test it. Ask for something in their voice and check it against the real thing.
> Submit a short summary of what you fed it and why you chose those sources.
> Submit to: bootcamp.paretotalent.com/homework
> Remember to: Post your homework in your assigned #Homework. · Share one thing you liked abou[t ...] (the slide text is cut off here)

Clarifications Ivan gave in Q&A:
- "By 3 different sources, I don't mean 3 posts from Facebook. I mean Facebook, Instagram, podcasts."
- The deliverable format is free: a project link, a Drive folder, a PDF, a video walkthrough. "If you will do it in 100 [words], I'm cool."
- Focus on extracting voice. The test output can be a Facebook post, an email reply or a blog post.
- Quality over volume: "not only trying to fit as much, but also trying to fit quality."
- Any tool is allowed: "If you will find a better way to do something, do it."

## Final project hints

- "In the very end, when we'll be having the final project, one of the things that I will ask you for is your chats with AI that you'll be using." Trainees must show they used AI properly.

## What comes next (from slides and transcript)

- **Day 3 (tomorrow)**: connect Claude Desktop, Claude Code/Cowork, Fathom, Google Drive (connect, don't download), WisprFlow and a markdown editor (Obsidian/VS Code) into a **Second Brain** system. It will include "more ways to mine for context ... and some creepy ways as well."
- **Day 4**: "the real build" for agentic work.
- A dedicated project-management class is coming later (projects vs. tasks).
- Apify will be covered in more depth later.

## Related
- [[ivan-bunin|Ivan Bunin]] · [[kasim-aslam|Kasim Aslam]] · Amparo Linares · [[right-hand-program|Right Hand Program]] · Pareto Bootcamp · [[two-layer-second-brain|Second Brain]] · [[context-engineering|Context Engineering]]
