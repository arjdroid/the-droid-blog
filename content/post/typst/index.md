+++
draft = "true"
author = "Arjdroid"
title = "Thoughts on Typst"
date = "2025-09-30"
description = "It's just better."
tags = [
    "school",
    "typesetting",
]
categories = [
    "school",
    "typesetting",]
series = ["School"]
aliases = ["Typst"]
image = "setup.jpg"
+++

For a couple years now I've been a vocal advocate of using the Typst typesetting system.

It is such a joy to use Typst for all of my coursework. I have tried both, LaTeX and Typst extensively. In all manner of environments, from OverLeaf (and the excellent Typst Web App) to VSCode, to Zed / neovim and zathura (the only PDF viewer I have found which supports decent vim bindings, and live refresh while still maintaining your exact position on a page; as a bonus, its FOSS and a pretty healthy one at that).

Typst makes me enjoy doing my coursework, because doing mathematics becomes even more fun. Seeing a beautifully typset document born re

I have even taken an undergraduate freshman seminar at UCSD last quarter, _PHYS 87_, with Professor Benjamin Grinstein, it was all about LaTeX. I think the system has plenty of benefits over alternatives like Google Docs, and heaven-forbid Microsoft Word (I have a decade of experience in Cambridge International Primary+Secondary Education Information and Communications Technology forcing Word down my throat, I am well aware of its advantages and disadvantages -- /*emdash*/ Mail Merge anyone?).

TeX especially, as devised by Knuth, is oh-so elegant with its macros. Then LaTeX has come along, and you're telling me I need to download gigabytes of packages from a random CTAN /*citation needed*/ in order to compile the simplest documents? Even with homebrew, though the installation process might be smoother, you're still downloading so much, otherwise you forego weird little features if you stick with a minimal installation (during the seminar, I was unable to have emojis in my documents at one point due to not having that latex particular package). Typst just has a more modern and elegant package ecosystem.

I also think that if you come at it from a modern programming background, then Typst makes a lot more sense intuitively as its more derived from markdown and popular programming languages with `c`-like syntax as opposed to the more math-intuitive and percentage-sign-laden syntax of LaTeX.
Initially, I did actually feel that typing math out in LaTeX was faster than Typst, especially if trying to keep up with lectures. However, the actual document typesetting is more of a pain. And, as I've gotten more accustomed to the niceties of Typst with such convenient functions like `cases()`, I really appreciate that I can typeset formulae faster than I can write them on paper or on my reMarkable in Typst. It's really great to use in Obsidian with the plugin `wypst` as well, although I have a gripe that the plugin hasn't been updated in a _while_ and is behind on the latest Typst features, maybe I should make a pull request.

Also, Typst is really performant. During my seminar, as we progressed through the class I could feel the agony of waiting for my saved changes to be updated by `lualatex` when using the `watch` command on my work.

The error messages in LaTeX are so esoteric, as compared to Typst it's not even comparable.

As an aside, I don't like how the abuse of Generative AI by my peers has made it so that I am forced to use Google Docs (or Word, basically the only two cloud-based Document Suites widely available and already paid for by my tuition) in order to have a third-party controlled edit-history paper-trail of working on my essays continuously over long periods of time. I will say it does force me to have better writing practices like starting early and starting often instead of last minute panicked work. However, I don't enjoy using Google Docs that much. It is still finicky, though not as much as Word, on non-printable characters (I often do `cmd-shift-p` to see them and make sure my line breaks are proper...), and don't get me started on the alignment of tables.
When doing my IB Chemistry Coursework, I really enjoyed the deterministic behaviour of Typst's tables, to include images, text, and chemical formulae without having to worry about whether my alignment would be set off was such a relief, not to mention the document as a whole. It was really handy when optimising stuff like page count (because, for some reason they used to enforce page limits instead of word limits???)
I guess for turning in essays and term papers in the humanities, it isn't too bad that I have to use Google Docs because I can still have mostly deterministic behaviour when using Styles and carriage-returns, but its a little annoying to not have the keybindings I want. I love that macOS has proper emacs-bindings like `ctrl-a/ctrl-e` to go to the start/end of a line, it inherited this from NeXStep /*citation needed*/, and is something I intend to use GTK rules to replicate that beautiful keybinding behaviour on GNOME, though thats another aside. \
Still, I want my Vim bindings in Google Docs, so I might be on the cusp of shelling out for a license for vimfordocs, but I'll wait till I have a paper due and use the free trial before I go down that path.

git + Typst/LaTeX is not really enough because though I may PGP sign my commits and push them to GitHub or my School's BitBucket, I guess someone could still /*futz*/ mess with forced re-writes of git history and I don't really want to be stuck in a position where I'm being questioned about that.

// TODO: import points from emails I've sent out
// gotta have one of those beautiful tiling_wm+macos+zed+zathura screenshots, heck my GNOME config looks great too, should check out some extensions for more beautiful screenshots.

Over my years of experience in converting others to such a typesetting system, I have noticed some observations:
- It is nigh impossible to convince someone who has already accepted the compromises (and benefits) of LaTeX, especially professors and researchers that have been using it for decades, to even check out Typst.
  - I think this is completely fair, especially given that they have already invested the time to optimise their workflow, and the network effects of LaTeX (at least in CS, Physics, and Math), being the de-facto format in which papers are submitted to journals for review, etc.
  - There have been efforts to convince the ArXiV to accept papers in `.typ` but these have gone nowhere
- It is far easier to convince classmates being introduced to LaTeX for the first time, that Typst is a far superior alternative to pick up and get started with.

Still, as I progress on in the years, I know I will probably have to adapt to being productive with LaTeX too because that is what the _overwhelming_ majority of peers use, and would be expected of me if I were to go into research, etc. `pandoc` is pretty neat for converting between LaTeX and Typst, but its not perfect, and its algorithmically-produced typesettings are often un-intuitive, overly riddled with backslashes (Typst saved my pinky finger from that too)

For personal use, and possibly even as a static site generator, I think I will prefer Typst.
