+++
draft = "true"
author = "Arjdroid"
title = "On AI and Programming"
date = "2025-12-30"
description = "Did Claude Code make me an AI Bro?"
tags = [
    "technical",
    "programming",
    "ai",
]
categories = [
    "technical",
    "programming",
    "ai",
]
series = ["ai"]
aliases = ["ai-programming"]
image = "claude.png"
+++

blog post
> did Claude Code make me an AI bro? [[AI and Programming]]

A couple months ago, someone important to me asked me a deceptively simple question, "what are your thoughts on AI?". I wanted to give them the well-thought-out and nuanced answer they deserved, but the best I could muster up on the spot was something along the lines of "I don't really know what to believe", and "the hype cycle is not sustainable". 

This blog should be what I said then.

Over the past couple of months I've been trying to figure out how I should be feeling about this, I mean its been 3 years since the release of ChatGPT (I know AI has been a hot topic for decades longer than that).

Almost since day 1, I've had a subscription to ChatGPT Plus. For the longest while, I've been off and on about actually admiring it.

The most prevalent use I've seen thus far is for academic dishonesty. And I've been squeamishly running from AI in almost a luddite fashion just to get away from that association. In trying to run away from it, intentionally only doing things by hand as far as possible, I was making the same mistake (in mindset) as my fellow college students; I was only seeing gen AI, llms, whatever you want to call it, as a way to cheat on homework [[#tangent 1]]. 

After getting home for winter break a couple weeks ago, I finally decided to switch that almost 3-year long subscription from ChatGPT Plus to Claude Pro. I wanted to use Claude Code after hearing so much hype about it on HackerNews. (I know I could have used Codex or Copilot CLI, but first mover advantage, the name and trust of a brand is really powerful for humans even if you're aware of it)
> could make the tangents a little shorter OR actually I like this idea better: make it a footnote!!!!

What did I use it for? I had some projects that had been sitting on my mind for months, but there was always another homework assignment for me to work on, or exam to study for, or big rock for me to climb. Still, I would read up on docs, occasionally a new Chat window that would inevitably disappoint me, etc. but never really getting started on the actual code itself. Claude Code made it so _fun!_. I was able to get into a new stack, piece together components I thought would've been rather complex, and just ship something. It was quite quick and easy to get 80% of the job done, the only limitation really is how much I _care_ for that last 20%. [typcraft](https://typcraft.nxtdroid.win) is live now. There are still a lot of things I could do to make it nicer, but my attention has already moved on (there's always something more fun to do, especially when it comes to anything that's not school or work)

I had a pretty decent idea of what I wanted to get done, just not the actual mechanical writing of code. The back and forth conversation with Opus 4.5 is very productive and allowed me to steer it away from unnecessary complexity, I wanted to keep the code as _simple as possible_.

>seems performative again ahahahaha

It's crazy how good Claude Code is, and how much better it could be. This [talk]() by Steve Yegge and Gene Kim is really good, and paints a picture of what the next couple of months could look like in AI-driven development.

...

Recommended Reading:
- Thinking with Machines, by Vasant Dhar
- (If you're thinking of going into the software world) Vibe Coding by Gene Kim and Steve Yegge
- Dune, "thou shall not make a machine to _counterfeit_ the human mind" or something along those lines, its been getting really popular haha 
- Some essays that are really pleasant:
	- On Machines of Loving Grace

> I have a scope problem, need to limit the scope of these posts man; or more accurately, decisively stick to a scope. Decide what I will and will not address, instead of trying to half-assedly have it all.
###### tangent 1
I, ostensibly, don't want to cheat on homework because (in my mind) I'm paying boatloads of money to learn rather than get a degree. However, I can totally see why the incentive structure of _a college degree_ and the _job market_ has made passing off one's assignments to a rational choice. If you see the homework as something in the way between you and a degree which would lead to a job, then it may be understandable what you're doing. I am trying to be a hipster, and this is vaguely performative – especially by penning it down in a blog post that will be seen by very few humans – but its along the same lines as cutting off social media and trying to read more for me; I don't really care what other people are doing, but I don't want it for myself. Perhaps its to the same extent with drinking (wherever its legal) and sugar and all those other things too; I know it brings a lot of joy to a lot of people, but I don't want it.
> this tangent might be out of scope...

content sync from my Obsidian vault:

blog post
> did Claude Code make me an AI bro? [[AI and Programming]]

A couple months ago, someone important to me asked me a deceptively simple question: "What are your thoughts on AI?". I wanted to give them the nuanced answer they deserved, but the best I could muster on the spot was something along the lines of "I don't really know what to believe". 

This blog should be what I said then.

Over the past couple of months I've been trying to figure out how I should be feeling about all of _this_, I mean its been 3 years since the release of ChatGPT^1.

> footnote 1: I know now that AI has been a hot topic for decades longer than that, although I've only been sapient for less than a decade

 I've had a subscription to ChatGPT Plus since almost Day 1, yet for all that time I've been off and on about actually using it. Sure, sometimes it was neat to ask it to write a shell script to automate a task, or to explain where I went wrong on a math / programming problem. 
 
 Yet, in terms of actually 'doing' all the cool stuff AI bros say LLM's can do – from replacing SWE's to giving nuanced research reports – I've often been left disappointed. However, now I'm a lot more bullish, what's changed?

Focusing on programming first, part of that disappointment had roots in the limitations of LLMs. A year ago, LLMs were still struggling to one-shot short pieces of code that I requested. This was especially the case for more niche stacks whether it be Svelte, Rust, or Typst. There was just less training data in these as compared to Node or Python which is what most LLM evangelists use. 

Nowadays, Claude Opus 4.5 / Gemini 3 Pro / GPT 5.2 Thinking are decisively _good_ at one-shotting code that compiles and does what I ask for. Even relatively obscure languages like Elm are now amenable, perhaps even preferable – more on this later. There is more training data, better fine-tuning, and improvement in model architecture.

Part of what's changed is also that I've grown in my own knowledge and understanding of LLMs and the tasks I try to get them to do. In personal pursuits I'm often distracted easily, so going to university for a CS degree has helped me actually learn how to structure and write programs. This is really useful as there are a lot of things – like data structures and algorithms – that I didn't go out of my way to pick up while self-learning by watching youtube videos and making random stuff. 

A better understanding of programming has definitely improved my ability to recognise when an LLM is going in a direction that isn't good. This is why 'vibe coding' in the original sense of the term (blindly trusting LLM output and letting it lead the way) never really worked for me. My own understanding of the codebase and problem space was too limited to use an LLM as a force multiplier.
> Claude code has changed this in my eyes, will write about that below

Over the past year and in my physical surroundings, the most prevalent and 'successful' (depending on how you view it), use of LLMs that I've observed is people skirting their university coursework. I've stopped keeping count of how many people I see in lecture halls, libraries, coffee shops, etc. pasting whole blocks of ChatGPT (it's always ChatGPT) output directly into Canvas, Google Docs, or VSCode. It makes me a little sad, but I don't care too much what other folks do with their time and money if it isn't directly harming other people.

Still, these observations, and fear-mongering from school staff about plagiarism, made me a bit of a Luddite. I wanted to actually learn what I'm doing and avoid the stench of dishonesty so I almost completely avoided using LLMs altogether. In doing so, I was making the same mistake as my fellow college students: I was only seeing AI as a tool for academic dishonesty, rather than something far more powerful.

> footnote 2: One of my professors gave a really compelling pragmatic argument for avoiding dishonesty on coursework that stuck with me, it was something along the lines of this: Imagine you are setting out on the pursuit of physical fitness, one of your tasks is going to be running. Running is a pretty inefficient way to get from A to B, especially at longer distances like 5km. Taking a car to go 5km would be a lot faster, more convenient, and comfortable. Yet, if your goal is to get fitter, 

Also, the relative success of LLMs at making people pass college with decreased effort gives insight into the future of AI use in knowledge work. With a lot of these assignments, especially in STEM majors, the task is very well defined and the steps to solve the problem are already laid out – if not already in the training data. There is also a clear idea of what solutions are right and wrong. This is an ideal situation for LLMs to score well.

After getting home for winter break a couple weeks ago, I finally decided to switch that almost 3-year long subscription from ChatGPT Plus to Claude Pro. I wanted to use Claude Code after hearing so much hype about it on HackerNews. (I know I could have used Codex or Copilot CLI, but first mover advantage, the name and trust of a brand is really powerful for humans even if you're aware of it)
> could make the tangents a little shorter OR actually I like this idea better: make it a footnote!!!!

What did I use it for? I had some projects that had been sitting on my mind for months, but there was always another homework assignment for me to work on, or exam to study for, or big rock for me to climb. Still, I would read up on docs, occasionally a new Chat window that would inevitably disappoint me, etc. but never really getting started on the actual code itself. Claude Code made it so _fun!_. I was able to get into a new stack, piece together components I thought would've been rather complex, and just ship something. It was quite quick and easy to get 80% of the job done, the only limitation really is how much I _care_ for that last 20%. [typcraft](https://typcraft.nxtdroid.win) is live now. There are still a lot of things I could do to make it nicer, but my attention has already moved on (there's always something more fun to do, especially when it comes to anything that's not school or work)

I had a pretty decent idea of what I wanted to get done, just not the actual mechanical writing of code. The back and forth conversation with Opus 4.5 is very productive and allowed me to steer it away from unnecessary complexity, I wanted to keep the code as _simple as possible_.

>seems performative again ahahahaha

It's crazy how good Claude Code is, and how much better it could be. This [talk]() by Steve Yegge and Gene Kim is really good, and paints a picture of what the next couple of months could look like in AI-driven development.

...

Recommended Reading:
- Thinking with Machines, by Vasant Dhar
- (If you're thinking of going into the software world) Vibe Coding by Gene Kim and Steve Yegge
- Dune, "thou shall not make a machine to _counterfeit_ the human mind" or something along those lines, its been getting really popular haha 
- Some essays that are really pleasant:
	- On Machines of Loving Grace

> I have a scope problem, need to limit the scope of these posts man; or more accurately, decisively stick to a scope. Decide what I will and will not address, instead of trying to half-assedly have it all.

The importance of people?

Ok, I will limit the scope of this one to just AI and Programming for now. Keep the more philosophical aspects and broader societal implications out of it.

outline:
- introduction
- switch from gpt to claude
- what did I use it for
	- when is it good
	- when is it not as good
- what's next
	- multiple agents? yegge's oxygen analogy
> succinctness of writing
what are the ideas I want to convey?

For a while I haven't "seen the light" with AI. I thought it was just going to be another incremental thing, and that people are using it as a crutch for cognitive decline. I think that view isn't entirely incorrect, but it is really limiting the scope of impact, and *scale*. Sure, there is a hype cycle. Sure, there are companies getting funding right now, for perhaps frivolous purposes. Still, it is not going to just "go away" as some people might wish. Things are going to change. And I would like to be on the right side of that, although I don't know what *that* looks like. Software is the first peek into this. Shipping stuff is going to get a whole lot easier. People have always been writing bad code; writing bad code is easy, but not necessarily simple. Now, we have an opportunity, to spend less time hand-writing code (a thorough understanding of a codebase is still necessary and central to the objective), and more time thinking about what we want programs to do.
###### tangent 1
I, ostensibly, don't want to cheat on homework because (in my mind) I'm paying boatloads of money to learn rather than get a degree. However, I can totally see why the incentive structure of _a college degree_ and the _job market_ has made passing off one's assignments to a rational choice. If you see the homework as something in the way between you and a degree which would lead to a job, then it may be understandable what you're doing. I am trying to be a hipster, and this is vaguely performative – especially by penning it down in a blog post that will be seen by very few humans – but its along the same lines as cutting off social media and trying to read more for me; I don't really care what other people are doing, but I don't want it for myself. Perhaps its to the same extent with drinking (wherever its legal) and sugar and all those other things too; I know it brings a lot of joy to a lot of people, but I don't want it.
> this tangent might be out of scope...

