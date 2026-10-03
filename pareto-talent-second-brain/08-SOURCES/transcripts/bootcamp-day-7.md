---
type: source
source_type: transcript
title: Pareto Bootcamp Day 7
captured: 2026-10-03
origin_url: https://drive.google.com/file/d/1XFZYYOX63HRNiLQZFaG_RHw44GbGdFGf/view?usp=drivesdk
slides_url: https://docs.google.com/presentation/d/1captqyPLlJCS4VkWITXWK1eiBOEKNqb77elPow8JOLY/edit?usp=drivesdk
speakers: [Ivan Bunin, Amparo Linares, Candela Copello]
participants_qa: [Christian Krieghoff, Amilcar Garcia, Melina Mazzoleni, María Paz Echandi, Gervasio, Luis De La Zerda, Joaco Faya, maria elena vallejos, Sandra Denis, Cristina Lopez, Juan Nonis, Paulo Adrian Miranda Rojas, Gonzalo Preis]
tags: [bootcamp, day-7, ai-image-generation, ai-video, voice-cloning, ad-creative, b-roll, video-editing, canva, right-hand-training, matching, 2-6-2-framework]
status: draft
---

# Pareto Bootcamp Day 7 — AI Image & Video Generation

> Source files: slide deck "Pareto_Bootcamp_Day7" and "Pareto_Bootcamp_Day7 - Transcript.txt" (Zoom WEBVTT, ~1h54m). Titles confirm Day 7. Both read in full.
> Audience: bootcamp candidates training to become Pareto "Right Hands" (Latin America-based executive assistants). This is a skills day (creative production), not a sales day, but it carries several proof points, team stories and the matching model (2-6-2) relevant to the [[right-hand-program|Right Hand Program]].

## Topic of the day
AI image and video generation for *commercial* creative: on-brand images, ad creative, AI B-roll, AI avatars, voice cloning, and fast AI-assisted editing. Slide framing: "Today is the raw material. Tomorrow is the system." Day 8 = personal brand, content planning, scheduling, marketing structure ("what should we post, and when" is tomorrow; "how do I make this exist" is today).

Recurring thesis from Ivan: always think about the **end goal / commercial intent** — "The end goal is not just to generate some image. The end goal is where this image will be used, how it will be used, how it will be perceived by the end user." Generating funny images with no commercial intent "prevented a lot of people from building something that's actually useful."

## Session outline (slides "Today's Plan" + actual flow)
1. Prompting for on-brand images, and why you iterate instead of regenerate (Ivan)
2. The same tools, aimed at ads: what actually changes (Ivan + Amparo, Canva demo)
3. Text-to-video tools, and voice cloning for narration (Ivan: HeyGen, Higgsfield, ElevenLabs)
4. Candela's toolkit: cutting, animating, editing (OpusClip, Riverside, OpenArt, Claude projects, Claude Design, Claude Code video editor, DaVinci)
5. Three live demos: image, video, a real edit
6. Q&A (B-roll libraries, voice-to-voice, final project/matching = 2-6-2, lip sync, laptop power), homework, job announcement

## Frameworks and models taught

### 1. Iterate, Don't Regenerate ("the one rule that saves everyone time")
- Slide: "The first image is a draft, not a failure." Refine the same generation: adjust the lighting note, swap one word, ask for a variation. "Starting over from a blank prompt throws away everything the model already got right."
- Analogy (slide): same as Day 5 vibe coding — "you are the architect, the model is the builder. Nobody scraps the whole house because one wall is in the wrong place."
- Ivan's decision rule: if output is "not even close" -> go back and redo the initial prompt. If it is close but style is off -> iterate on the same image; "Don't use the same prompt and just click send."
- Callback to Day 6: the Kasim image was "completely horrible" at first; adding materials and guidance fixed it.

### 2. On-brand image prompt: feed it the same three things, every time
1. **Section description** — what the image is for (hero background, testimonial avatar, product shot, social banner). "The platform will dictate the output."
2. **Style guide** — brand tone in a sentence; fonts, colors, vibe/energy. Can be saved as a reusable preset (e.g., in Claude Design, Gamma). Ivan: "This is context... what will root your AI into something real... without that, all of the images... will feel like AI fluff." Same idea as the second brain.
3. **Palette screenshot / references** — from coolors.co or CSS Peeper (Day 5). "Colour is the fastest thing to get wrong and the easiest thing to just show it directly." Reference images act as palette: "I want this vibe, but with this face."

### 3. Deconstruct-then-reuse (reference ad -> master prompt)
1. Find inspiration that already works: Facebook Ads Library (facebook.com/ads/library — e.g., see what "Harmozi" [Hormozi] is running and spending on), Pinterest saved ads, Ideogram/Midjourney community prompts.
2. Paste the reference into AI: "analyze this image and deconstruct it. What is the style, how it works... build it out as a prompt that I would be able to reuse."
3. Save the result ("visual deconstruction" + "reusable master prompt") as an artifact to reuse.
4. Generate with the subject's likeness (e.g., Kasim) in the reference's camera angle; keep feeding references until likeness is right.
5. Finish in Canva: copy colors from the reference, identify font (What's the Font), use Canva pre-assembled text blocks ("proven font pair"), duplicate image + remove background to get subject-overlapping-text effect.
- Formula stated: "AI plus templates equals a good image."
- Unusual camera angles (e.g., shot from below) are scroll-stoppers: "that's why we stop scrolling."

### 4. Batch ad-creative workflow (Amparo)
1. Use the second brain to identify audience/target customer and divide their pain points.
2. Generate a prompt per pain point / "every single angle" — "a bazillion prompts."
3. Run prompts in batches across many parallel ChatGPT chats (she had ~10 open) because generation is slow.
4. Ask for variants of winners (Ivan flagged one that "worked pretty well" -> variants: sunset, night at an airport, daytime).
5. Translate what already works (screenshots of ads -> "build me a template for this").
6. Assemble in Canva; once a template works, create variants (swap image, colors, fonts) to test. "We did hundreds of different of these."

### 5. Best B-roll library hierarchy (Ivan, answering Christian)
1. Your own B-roll library (client filmed doing things: meetings, computer work, gym). "The best B-roll is your own. It's not stock."
2. AI of your own — "stuff that you wish you had recorded, but you haven't" using the character's likeness.
3. Free stock (Pexels) — problem: mismatched color grading; must color grade individually or "it will look like a mess."

### 6. A-roll vs B-roll (definitions)
- A-roll: main voice/talking footage. B-roll: silent clips placed on top of A-roll to illustrate a point; "usually quick shots... five seconds, 10 seconds."

### 7. Candela's B-roll pipeline (Claude project "Monet")
1. Drop the transcript into a pre-set Claude project (knows her process + a knowledge base on "how to think cinematically").
2. Claude pitches B-roll ideas; she picks (e.g., "I like the 7 and 8").
3. Claude writes still-image prompts; iterate on still images first (cheap) "until it nails it."
4. Animate the approved still into video (OpenArt).
5. Style is embedded in the project (e.g., an "impressionist, oily painting" style) for consistency across all Kasim videos. "You can tell it's AI. But I don't want to hide it anyways."
- She had Claude write the project instructions itself: told it her process and frustrations.

### 8. Hooks x bodies ad matrix
- For advertising, produce many hooks and many bodies and match them "to have, like, a net of content." Candela automates matching with Claude Code (folders of e.g. "unhinged Nuno hooks"; prompt: "Put these videos together, put subtitles, and animate them"). Claude Code transcribed without "a single word" error; added timed sound effects and music.

### 9. Realistic Right Hand editing scope (minimum viable edit)
- Ivan: as a Right Hand, most tasks are "cut the silences off, add the transcript, add one B roll done." "Remove the silences, remove me swearing a couple of the times and add some light music in the background and then titles and send it to my Instagram. Done." Extra mile = motion graphics via Claude Design.
- Commercial editing is "very much simplified right now with AI"; creative/film editing is a different topic — "one is not killing another."

### 10. The 2-6-2 framework (Kasim's; used in matching) — high relevance
- Ivan: "this is something that Cassin [Kasim] developed as a 262 framework... something that, again, we use in the background."
- Of 10 things shown: **2** you'll be "complete trash" at; **6** you'll do okay; **2** "you will be the best at."
- "Our job is to try to match you, so you will not be doing that stuff [the bad 2]. So you will do stuff that you're actually good at, that you actually enjoy."
- Matching process: "we are analyzing what you're actually good at, and then we are matching you with an entrepreneur that needs that." Example: weak at websites but good communicator / project management / images -> "chances are you are a social media manager" or client-facing role.
- "You're not expected to do everything. My job is to give you all of the different things that you can stuff into your belt."

### 11. Tools-must-pay-for-themselves rule
- "If you are not able to make $1,000 with these videos, then you're doing something wrong." "All of these tools... should pay for themselves with the stuff that we actually generate."
- AI lets you "prove the concept" and "decrease the exposure in budget to do some crazy ideas," then scale manually.

## Numbers, stats and proof points
- ~**$10,000** ad spend (across campaigns) on one AI+Canva ad Amparo showed; "it really did generate us some results, some registrations" for workshops in the **VibeCode Incubator**. "We actually go ahead and eat our own dog food."
- ~**$1,000** in Higgsfield credits for all the AI Nuno hooks and bodies across multiple workshops; compared to "a videographer, a couple of days of shooting... it kind of pays for itself."
- Higgsfield demo: 6-second, 16:9, 1080 clip on Seedance cost **72 credits**; Ivan had "a couple thousand"; free tier "like 10 credits."
- ElevenLabs professional clone: feed ~**2 hours** of clean audio; Ivan already has "**14 hours** of me talking" from the bootcamp.
- Ivan worked as Kasim's executive assistant for **4 years**.
- Ivan's homework raw video ~**2 minutes**; "usable... probably, like, 15 seconds."
- Canva slide stats: **1.6M+** templates across **1,000+** design types; **4.7M+** free stock media; free Brand Kit capped at **3 colours**.
- HeyGen: **1,100+** presenters (slide). Higgsfield: **50+** camera movements (slide).
- Background removal manually used to take Ivan "20 minutes per photo."
- Claude Code workshop ad VO: "Four days live starting June 1."
- "All of our team from Pareto Talent is from the same Bootcamp. Candela is coming from the same Bootcamp."
- Kasim (fake message used as illustration, Ivan admits "this is me messaging myself, custom is fake"): "we need an editor for Leverage School." Ivan: whoever edits best may get a job by end of bootcamp; would work with Agustina primarily.

## Stories (2-4 lines each)
- **Kasim image redo (Day 6 callback):** first AI image of Kasim was "completely horrible"; adding reference materials and guidance turned it into something useful — proof of iterate-don't-regenerate.
- **Nuno old-computer ad:** instead of asking Nuno to find an old computer for a photoshoot, Ivan generated the scene with AI; pre-2021 it would have required a studio or expert Photoshop.
- **AI Nuno hooks:** fully AI-generated videos of Nuno with a voice clone (Higgsfield Cinema Studio + ElevenLabs) for Claude Code Workshop ads; Ivan has met Nuno in person and says "it sounds like exactly the same... it sounds better here than he does on YouTube." Hooks heard: "What loses most people building their first app isn't the code."; "There's one skill under every AI tool. Nobody teaches it."; "You've rented a car you'd never driven. And drove it off the lot anyway."; "Third weekend, you promised yourself you'd finish the app."; "You can keep using AI like a slightly smarter Google, or you can learn to build with it."
- **Pareto clay figures:** Ivan made all Pareto Talent website images present parts of the offer using clay figures, for reusable branding; "Now I kind of regret this." Point: illustrate the customer's pain, not "one, two, three."
- **Ivan's design-studio photo:** dropped an old low-res photo into ChatGPT to upscale; "a lifesaver for majority of personal brand stuff."
- **Mad Men contrast:** big-concept shoots (model dropping fries, splash) are cool, but "usually we need ads tomorrow" — AI first, creativity on top.
- **Ivan as bottleneck:** video creation (lights, cards, file transfers) is "a pain in the butt"; Ivan is teaching Ampy and Gaspar so "we don't have to record the videos all the time."
- **Candela:** full-time video editor/motion graphic designer, came through the same bootcamp; uses Premiere and After Effects daily; Claude Design animation would take "a couple of hours" in After Effects.

## Pain language and objections (verbatim)
Founder/operator pain (Ivan, as founder):
- "Usually we need ads tomorrow. Because, hey, we decided that we're running this workshop, like, let's do some ads, right? Usually you won't have enough time for that stuff."
- "That allows me to remove a lot of the things that where I'm the bottleneck like creating the videos and all that it takes a lot of time."
- "Setting up all of the light equipment then having all of the cards transferring files between here and there it's a pain in the butt."
- "A lot of these older photos, they're, like, look horrible, and you just want to lift them up a little bit."
- On the use case: "Without Kasim having to do anything" — "we can generate videos for [Kasim's] social media or for ads, which will sound like [Kasim]... without [Kasim] having to do anything."
Candidate concerns/objections:
- Melina: "the input is so huge that it will take some time for me to take in everything."
- Joaco: "we have to spend credits on these platforms. Is there any way that we can make this free?"
- María Paz: lip sync "sometimes it looks a little bit odd to see."
- Luis: Google Flow "time limit for the duration"; voice "shifted to another kind of voice."
- Ivan on AI-everything editors: "you're given all of the keys to AI and just tell, hey, like, just do something... the result might not be as predictable or as customizable."
- Ivan on AI misuse: "the use case that I see, unfortunately, majority of people having with AI is memes."

## ICP / offer signals (for the Right Hand Program)
- What clients actually need: "usually, again, we don't have clients that need hardcore app development or stuff like that. Usually, again, our clients need real right hand."
- Right Hand creative scope per Ivan: cut silences, captions, one B-roll, light music, post to Instagram; produce ads with founder's likeness and cloned voice so the founder doesn't record.
- Example client/founder types implied: founders running workshops/masterminds/one-on-one support (Kasim), e-commerce clients with products (Higgsfield "elements" for consistent product in UGC).
- Matching promise: match Right Hand strengths (2-6-2) to the entrepreneur's needs.
- Pareto team is bootcamp-sourced (Amparo = Ivan's right hand; Candela = video editor; Gaspar, Agustina mentioned).

## Jargon and terms
- **Right hand** — Pareto term for the executive assistant (Amparo = "my right hand").
- **Iterate, don't regenerate** — refine the same generation vs. new blank prompt.
- **Section description / style guide / palette screenshot** — the 3 inputs for on-brand images.
- **Master prompt / visual deconstruction** — reusable prompt derived from analyzing a reference image.
- **Magic prompt** (Ideogram) — AI expansion of your prompt; **Seed ID / Style Creator / Midjourney styles** (Midjourney) — reusable styles.
- **A-roll / B-roll / AI B-roll** — main footage vs. illustrative overlay clips; AI-generated overlay.
- **Hooks and bodies** — ad openers and main sections, mixed and matched.
- **UGC** — user-generated-content style video, via AI avatars.
- **SOUL ID** (Higgsfield) — keeps one character consistent across videos; **Elements** — saved consistent products/objects; **Cinema Studio**.
- **ClipAnything** (OpusClip) — finds strongest moments, auto-reframes 9:16/1:1/16:9. **Magic Hooks** (Riverside).
- **Color key** — keying out blue background on Claude Design animations (DaVinci free).
- **Talking head video** — person speaking to camera; Claude Design adds depth.
- **2-6-2 framework** — Kasim's skills distribution used in matching.
- **Second brain** — context store used to derive audience and pain points for ads.
- **Eat our own dog food** — Pareto runs paid tests on what it teaches.
- **Leverage School, VibeCode Incubator, Claude Code Workshop** — Kasim/Ivan programs referenced.

## Tools covered (as taught)
- Image: ChatGPT (general + photo enhancement/upscaling; Ivan "already pay[s]"), Ideogram (legible text in images; logos; community prompts), OpenArt (images + avatars; cheaper; free credits often on Discord; worlds/libraries for storytelling), Midjourney ("probably the best tool" for creative work; style blending), Higgsfield (all-in-one, many models incl. Nano Banana, Seedream, Seedance; "expensive"; "one of the best tools on the market").
- Finishing: Canva (Background Remover — paid; templates; brand kit; Dream Lab AI; elements like circles/arrows to highlight pricing), Photopea ("Photoshop online", Select Subject), What's the Font, Pexels.
- Video/voice: Google Veo-based tools (B-roll from text or photo), HeyGen (avatar studio; "not the best in the voice"), ElevenLabs (voice clone; voice changer; can connect to HighLevel to make calls), Higgsfield+ElevenLabs API for lip sync.
- Editing: OpusClip (paid, "by far the easiest"), Riverside (free tier; many entrepreneurs podcast on it), Descript, CapCut, DaVinci (free, color key), Premiere/After Effects (paid), Claude Design (on-brand HTML-based animations; Candela has a design system based on Pareto's website), Claude Code (drag MP4s; transcribe, cut silences, assemble, B-roll).
- Website use: loop animations (same start/end frame) and on-scroll animations from MP4s (AI Studio demo).
- Model advice: "don't focus on the models, try different ones" — they change monthly.

## Brand / voice notes
- Pareto website imagery uses **clay figures** illustrating offer parts (Ivan now regrets it).
- Candela keeps a **Claude Design design system based on Pareto's website** for on-brand animations.
- Demo ad copy used green text: "Don't let AI take your job." / "learn Claude code."
- Kasim's B-roll style: impressionist oily-painting look, openly AI.
- Slides' tone: plain, practical ("The first image is a draft, not a failure").

## Competitors / lead magnets / funnels
- No direct Pareto competitors named. Ads-research reference: Hormozi via Facebook Ads Library.
- Funnel-adjacent: workshop ads (Claude Code Workshop, VibeCode Incubator) built with AI imagery + Canva, $10K tested; online-workshop templates in Canva; hook/body ad matrices. Day 6 CRM email: default sender "mail.messagerndeliver.com" in the CRM.

## Final project hints
- Ivan reviews final projects first: "If your final project is crushing it, I don't care about the homework. If your final project is meh, then I'm checking the homework." Homework checked by next Wednesday when final-project review starts.
- Final project informs matching via 2-6-2: not expected to excel at everything.
- Homework images should relate to the landing page/website candidates are building (many built Kasim offers).

## Homework (Day 7, exact from slide)
"Generate, edit, and ship pieces of content: image & video."
1. Generate 2-3 on-brand Ad images using a description, style guide, and palette screenshot.
2. Download the sample video from Ivan promoting the Bootcamp.
3. Using AI, generate b-roll to add to your video, from either a text prompt or an existing image.
4. Edit all assets into one finished piece: use one tool to trim & put together your videos; add captions and some background music.
5. Submit the finished pieces, plus the prompts you used for both the image and the video.
- Submit to: bootcamp.paretotalent.com/homework. Post in #Homework; share one thing you liked in #General; share all finished assets in #Homework.
- Clarifications: images should illustrate a point on your website (e.g., "If your website is talking about a mastermind, show [Kasim] presenting to a mastermind"); video need not be fully AI or related to the site; bare minimum = "Just cut the silences, add two B-rolls, and you're done"; no length requirement; tools: CapCut, Riverside, OpusClip, Descript.
- Possible editing competition / job for best editor (Leverage School editor).

## Next day
Day 8: personal brand, social media strategy — "now, how do we use that to actually move the needle for them."
