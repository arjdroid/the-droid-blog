+++
draft = "false"
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

A couple months ago, someone important to me asked me a deceptively simple question: "What are your thoughts on AI?". I wanted to give them the nuanced answer they deserved, but the best I could muster on the spot was something along the lines of "I don't really know what to believe". 

This blog post should help me build _some_ of those thoughts, although I'm still trying to figure out how I should be feeling about all of _this_. I mean its been 3 years since the release of ChatGPT [1].

I've had a subscription to ChatGPT Plus since almost Day 1, yet for all that time I've been off and on about actually using it. Sure, sometimes it was neat to ask it to write a shell script to automate a task, or to explain where I went wrong on a math / programming problem. 
 
Yet, in terms of actually 'doing' all the cool stuff AI bros say LLM's can do – from replacing SWE's to giving nuanced research reports – I've often been left disappointed. However, I'm a lot more optimistic now about their capacity to yield productivity, what's changed?

Focusing on programming, part of my disappointment had roots in the limitations of LLMs. A year ago, LLMs were still struggling to one-shot short pieces of code that I specified. This was especially the case for more niche stacks whether it be Svelte, Rust, or Typst. There was just less training data in these as compared to Node or Python which is what most LLM evangelists use. 

Nowadays, Claude Opus 4.5 / Gemini 3 Pro / GPT 5.2 Thinking are decisively _good_ at one-shotting code that compiles and does what I ask for. Even relatively obscure languages like Elm are now amenable, perhaps even preferable – more on this later. There is more training data, better fine-tuning, and improvement in model architecture.

What's also changed is my own knowledge and understanding of LLMs and the tasks I try to get them to do. In personal pursuits I'm often easily distracted, so going to university has helped me actually learn how to focus, and think deeper. This is really useful as there are a lot of things – like different ways to structure computer programs – that I didn't go out of my way to pick up while self-learning by watching youtube videos and making random stuff that happened to be fun. 

A better understanding of programming has also improved my ability to recognise when an LLM is going off in a direction that isn't good. This is why 'vibe coding' in the original sense of the term (blindly trusting LLM output and letting it lead the way) never really worked for me. My own understanding of the codebase and problem space was too limited to use an LLM as a force multiplier, and the LLM wasn't all that familiar either. With tools like Claude Code today, and my knowledge only growing, I foresee AI as something I can leverage to do a lot more than I could without it.

Over the winter break, I finally cancelled my ChatGPT subscription and moved to Claude. I think this was long overdue, as Anthropic seems like a corporation more aligned with what I want to see in the future. Their CEO sure paints a beautiful picture, (see: [On Machines of Loving Grace](https://www.darioamodei.com/essay/machines-of-loving-grace)). But also, I really wanted to try Claude Code. After hearing so much praise and glaze on HackerNews and from friends, I was excited. Sure, I probably could have just used Codex, or Copilot CLI both of which I already had, but branding is really powerful.

I gotta say, Claude Code is *fun*. I set out to build a project I've had sitting on my mind for a little while. I had a good idea of what I wanted to build it in, how I wanted to structure it, and opinions on choices. The only thing I didn't want to do was the actual mechanical act of writing the code. Claude Code took care of that. In just a couple of sessions, it did great! I gave it details and it gave me code. Really, the only limitation was how much time I wanted to spend, although i guess that was always the limitation – its just a lot faster now! 

https://typcraft.nxtdroid.win is live right now, and quite barebones I admit, but it got the cool part functional: a real-time responsive `typst` compiler in the browser. Working in Elm, with Rust for the WASM bindings was refreshingly pleasant with my greater experience and smarter partner as compared to my previous attempts to do the same. Other folks' projects like [wypst](https://github.com/0xbolt/wypst), while good, were not that simple to get up and running even with the help of ChatGPT.

On a somewhat related note, the relative success of LLMs at helping people pass college with less effort [2] – dispiriting as that is – also gives insight into the future of AI use in knowledge work. Most homework assignments, especially in STEM majors, are well defined: the steps are straightforward, sometimes already in the training data, and right answers are clearly distinguished from wrong ones. These are ideal conditions for LLMs to provide correct output.

Similarly, Claude Code is a lot more pleasant than using the ChatGPT web interface because Claude is far better at planning the steps, and more efficient in responding to feedback to improve the quality of its code. I believe more restrictive and opinionated (in what passes as valid) programming languages – especially functional ones like Elm or Haskell – may be more ideal for programming with LLM assistance as compared to something like vanilla JS or Python. The stricter the type system, and the more informative the error messages, the better AI agents will be able to produce correct code.

It's crazy how good Claude Code is, and so promising how much better it could be. This [talk](https://www.youtube.com/watch?v=7Dtu2bilcFs) by Steve Yegge and Gene Kim is really good, and paints a picture of what the next couple of months could look like in AI-driven development [3]. Namely, the use of more and smaller AI agents specialising in singular tasks instead of the one big model taking care of everything as is the case right now.

For a while I wasn't "seeing the light" so to say with AI. I mistakenly thought it was just going to be another incremental improvement, and that people would use it as another crutch for cognitive decline. That last part isn't entirely incorrect, but my view vastly underestimated the *scale* and scope of the future impact of AI. Sure, there is a hype cycle that will follow the age-old trend of boom and bust. Still, it is not going to just "go away" as some people might wish. 

Things are going to change. And I would like to be on the right side of that, although I don't know what *that* looks like. Software is the first peek into this. Shipping stuff is going to get a whole lot easier. People have always been writing bad code; writing bad code is easy, but not necessarily simple. Now, we have the opportunity to spend less time hand-writing code, and spend more time thinking about what we want programs to do.

> [1] I know that AI has been a field of research for a handful of decades, but I've only been sapient for a handful of years thus far. My first forays into 'AI' were with trying to run GPT-2 and Stable Diffusion on my gaming PC during the pandemic, before OpenAI made things simultaneously more accessible and less open with the release of GPT-3 and ChatGPT.

> [2] One of my professors gave a really compelling pragmatic argument for avoiding dishonesty on coursework that stuck with me, it was something along the lines of this: Imagine you are setting out on the pursuit of physical fitness, one of your tasks is going to be running. Running is a pretty inefficient way to get from A to B, especially at longer distances like 5km. Using a car to go 5km would be faster, more convenient, and comfortable. Yet, if your goal is to get fitter, using a car utterly defeats that purpose: the desired outcome wasn't to get from A to B, it was to get the benefits that running 5km gives your body. The same applies to coursework.

> [3] https://www.youtube.com/watch?v=7Dtu2bilcFs

> This blog post [how-vibe-coding-killed-cursor](https://ischemist.com/writings/long-form/how-vibe-coding-killed-cursor) by [Anton Morgunov](https://ischemist.com) really provides concrete examples and advice for someone right now trying to write software with the assistance of LLMs.

Also, some more recommended reading:
- Thinking with Machines by Vasant Dhar
- Vibe Coding by Gene Kim and Steve Yegge
- Dune by Frank Herbert, "Thou shalt not make a machine to counterfeit a human mind."
