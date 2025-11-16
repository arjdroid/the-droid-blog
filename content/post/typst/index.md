+++
draft = "true"
author = "Arjdroid"
title = "Thoughts on Tantalizing typst"
date = "2025-11-16"
description = "A better way is so close, yet so far away."
tags = [
    "technical",
    "typesetting",
]
categories = [
    "technical",
    "typesetting",
]
series = ["typesetting"]
aliases = ["typst"]
image = "setup.jpg"
+++

For a few years now, I've been a vocal advocate of using the [typst](https://typst.app) typesetting system, an open-source toolchain that revolves around the `typst` compiler.

# The joys of typesetting

If you haven't yet discovered the joys of typesetting, I must say that typst is a most delightful introduction. That is really the best way for me to describe it: joyous. For those that are in the know, head over to the next section.

In high school and now college, I've made extensive use of typst to ensure a modicum of aesthetics in the presentation of my coursework. I could have done what my peers did, and use Docs, or god-forbid Word to complete the task. I probably would have procrastinated less. But using every time I type `typst` into my terminal, I feel a lot more enthusiastic about whatever I'm working on, whether it be an essay, a pset, or even a letter to a friend.

Have you ever felt frustration at Microsoft or Google for the clunky interfaces and occasionally erratic behaviour of Word and Docs? The main advocates for typesetting (with LaTeX) focus on the flexibility with which one can show equations. However, there is also an argument for having a deterministic workflow.

When you try to get the positioning of an image or table just right, only for it to be ruined because you wanted to change the phrasing of one of your sentences. Perhaps you're not as sufficiently plagued as I can be sometimes in an obsession over minutae, but you might still appreciate a faster way to type up your equations from coursework! 

# Why typst

If you're already a convert to the benefits of typesetting, chances are you're used to LaTeX, and you're saying to yourself, "LaTeX already does this!", and you'd be right.

I have used both, LaTeX and typst extensively. In all manner of environments, from OverLeaf (and the excellent typst Web App) to VSCode / Zed / neovim and zathura, and I can honestly say they're both great, but typst is just better.

It's soo faster to compile – which I know doesn't matter for a lot of people – but for my impatient self, the seconds-long wait between saving my document and waiting for _any_ LaTeX compiler to update the pdf is agonising. By contrast, `typst` prides itself in showing how few milliseconds it took to compile the very same document. It's implemented in Rust, with more modern, and more importantly, *_unified_* ideas about how to structure it.

> Zathura is the only PDF viewer I have found which supports decent vim bindings, and live refresh while still maintaining your exact position on a page; as a bonus, its FOSS with a pretty healthy community at that.

Secondly, the toolchain is just a lot nicer. I took a freshman seminar course on LaTeX to give it a fair shot, supposing that my individual exploration might not have yielded the blissful productivity others speak of. However, I found it to be exactly as I remembered: clunky, large and slow. I don't doubt that Knuth's original TeX was, and still is, buttery smooth.

However, the modern LaTeX ecosystem is burdened with so many random packages and huge file downloads; I shouldn't have to give up literal tens of gigabytes just to get basic documents going. It's 2025, we can do better.

I also suspect those coming from a modern programming background, pick up typst more intuitively as its more derived from markdown and popular programming languages with `c`-like syntax as opposed to the more math-intuitive and percentage-sign-laden syntax of LaTeX.

Initially, I did notice that typing math out in LaTeX was faster than typst, especially when trying to keep up with lectures. However, the actual document typesetting is far more of a pain. As I've grown accustomed to the niceties of typst with such convenient functions as `binom()` and `cases()`, I appreciate that I can typeset formulae faster than I can write them on paper or on my reMarkable in typst. 

> It's really great to use in Obsidian with the plugin `wypst` as well, although I have a gripe that the plugin hasn't been updated in a _while_ and is behind on the latest typst features, maybe I should make a pull request.

One thing I don't often see talked about, is that the error messages in LaTeX are so esoteric,it's not even comparable to typst.

I must concede that the LaTeX ecosystem is far more mature. With typst, there are breaking changes with new releases. I can't simply run `typst compile *.typ` on some of my first pieces of coursework I composed with it as there are minor errors I must fix beforehand. However, the error messages are actually human-readable so I can make those changes pretty easily.

# Trouble in paradise

Despite all its benefits, I think that the future offered by typst is like a mirage in the desert. The promise of a better, more productive oasis exists, but the harsh LaTeX-pilled sands around it erode at the perfection. Journals are quite wary of it. The ArXiV has explicitly stated (as of the time of writing) that they won't accept papers in typst. Labs and research groups all around my campus and those across the globe work in Overleaf. 

The sparks of resistance are bright, but they alone cannot light up the darkness. I have peers, even TA's that enjoy using typst, but they too have succumbed to the pressure of network effects. In group work, `pandoc` can only take you so far, though I have observed that many these days don't bother to write LaTeX, preferring to feed their multi-modal LLM of choice with equations scrawled on their iPads.

Much like julia and python, or c and rust, I don't think typst is going to follow in the footsteps of the Greek pantheon and kill off its precursor from before the turn of the millenium. I rue the day I must invoke `lualatex` once more, and count the seconds of my life slipping away as I await my slurry of backslashes and percentage-signs to produce less beautiful documents.
