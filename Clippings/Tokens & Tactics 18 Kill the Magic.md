---
title: "Tokens & Tactics #18: Kill the Magic"
source: "https://newsletter.brxnd.ai/p/tokens-and-tactics-18-kill-the-magic"
author:
  - "[[Noah Brier]]"
published: 2025-11-04
created: 2026-01-03
description: "Nic Hodges on building a Claude Code setup with 15 years of notes and why understanding how LLMs actually work reveals their real power."
tags:
  - "clippings"
---
### Nic Hodges on building a Claude Code setup with 15 years of notes and why understanding how LLMs actually work reveals their real power.

**Welcome back to Tokens & Tactics, our Tuesday series about how people are actually using AI at work.**

Each week, we feature one person and their real-world workflow—what tools they use, what they’re building, and what’s working right now. No hype. No vague predictions. Just practical details from the front lines. This week: **Nic Hodges.**

---

![](https://substackcdn.com/image/fetch/$s_!bA0-!,w_424,c_limit,f_webp,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F4ed1c025-8599-4e31-87e9-5bd53bef5bbb_1024x824.png)

Me in my dream workshop 😆

#### Tell us about yourself.

My name’s Nic Hodges. I live in Melbourne, Australia. I’m probably best described as a creative technologist. I’m a builder, sometimes that’s physical things, sometimes it’s digital things, and lately it’s about building an environment where creative people can do their best work.

Over the past 20 years I’ve worked in everything from industrial design to advertising to running digital media and innovation across agencies and media businesses. I ran [my own consultancy](https://blonde3.com/) for seven years, and since the middle of this year have been leading [Trout](https://www.trout.com.au/), a design agency. We have offices in Melbourne and Dallas, focusing on building brands in the trades, construction and home sector — and we only work with founders.

#### ChatGPT, Gemini, or Claude?

I’m 99% Claude. I have a rather convoluted Claude Code setup for my day-to-day work that’s accessing 15 years’ worth of markdown notes, and I find Claude understands that and responds to it in the most natural way.

In the early days when OpenAI and Microsoft were throwing around free API credits, GPT was definitely my go-to. But the tone of ChatGPT just doesn’t quite gel with me, and the variance between models seems quite high. Gemini is a similarly meh tone, except I do find Gemini is great for research and probably has less hallucination for real information gathering projects.

#### What was your last SFW AI conversation?

I just dropped these interview questions into my Claude Code terminal and started having a voice conversation, which resulted in the first draft of what you’re reading now. It was probably a ten minute conversation, and 90% of what you’re reading now came from Claude Code.

#### First "aha!" moment with AI?

The biggest aha moment for me was when LLMs stopped feeling like magic. The real breakthrough was understanding how these things actually work — transformers, token space, the underlying mechanics. Once I understood that, I could see both the boundaries and the real power. Understanding what the technology actually is, not just what it appears to do, lets you see where it’s powerful and where it’ll fail (or fool you into thinking it’s powerful).

#### Your AI subscriptions and rough monthly spend?

Personally, it’s just Claude Pro. I used to have a Perplexity Pro subscription but found I wasn’t using it enough to justify it. Within the studio we’re subscribing to a lot of different specialised tools, but for my personal workflow it’s really just Claude doing the heavy lifting.

#### Who do you read/listen to to stay current on AI?

People I’ll pretty much always read:

- [Simon Willison](https://simonwillison.net/)
- [Tim Lee at Understanding AI](https://www.understandingai.org/)
- [Import AI by Jack Clark](https://jack-clark.net/)
- [Gradient Ascendant by John Evans](https://aiascendant.com/)
- [Cognitive Resonance by Ben Riley](https://buildcognitiveresonance.substack.com/)
- [Ahead of AI by Sebastian Raschka](https://magazine.sebastianraschka.com/)
- [Melanie Mitchell](https://aiguide.substack.com/)

Most of these are deeper commentary and research around AI. For staying on top of the news, I rely on my friend Amin’s newsletter, [That AI Thing](https://thataithing.beehiiv.com/).

#### Your most-used GPT/Project/Gem?

My most-used “thing” is my CLAUDE.md file for my Claude Code setup — a spaghetti monster of various prompts I’ve built, stolen, or modified over the last few years that sits behind all my daily thinking and notes.

With [skills](https://www.anthropic.com/news/skills) coming to Claude Code, I’m now pulling those pieces out and turning them into discrete tools. I’ve asked Claude to tell you a few that it’s using regularly:

- **Evidence vs Story Separator** \- Anti-sycophancy tool that separates observable facts from interpretations (*Nic note: Claude built this skill after reading [this excellent research](https://arxiv.org/abs/2510.01395) on LLM sycophancy*)
- **Weekly Reflection** \- Guides end-of-week reflection with structured prompts, capturing wins, challenges, learnings, and things to get done in the next week
- **SOAP Meeting Transformer** \- Turns sprawling meeting notes into structured format (Subjective/Objective/Assessment/Plan)
- **Context File Maintainer** \- Monitors conversations for tasks, pattern shifts or timing markers and prompts updates to my active context file

#### The AI task that would've seemed like magic two years ago but now feels routine?

There’s obviously impressive stuff like nano banana and video models, but I’m not using those day-to-day. The thing that feels routine now but would’ve seemed magic two years ago is contextual memory — trusting the LLM to retain context and surface it reliably.

I frequently jump into my daily Claude Code chat and just tell it something I need to remember when it springs to mind. I’ve even built a shortcut on my Apple Watch so when I’m running and I think of something, I can send that idea and it goes to Claude.

Claude keeps track of everything I need to do. It hasn’t slipped up yet, and interestingly I don’t think that’s about LLMs getting better, it’s about the engineering around them.

#### Magic wand feature request?

I’m writing this by talking to Claude Code within a Tmux session in Terminal. It feels like playing a MUD game in the 80s. The technology capability here is insane, but the interface is agricultural. We have to build better interfaces.

#### If you could only invest in one company to ride the AI wave, who would it be?

If there’s one company that’s cornered the market on pouring the concrete slabs for all the data centres (and they’re not as overvalued as every other AI-adjacent company) I’d be backing those guys.

#### Have you tried full self-driving yet?

I’m in Australia, ask me in five years.;P

#### Latest AI rabbit hole?

Synthetic personas. I worked on this a few years ago with some market researchers and it seemed really promising, but the actual outcomes just weren’t valuable (despite feeling 100% right).

Recently, with some client customer research, I’ve been going deep again — trying to understand how to present data to an LLM so it can role play in ways that are actually beneficial for brand strategy, not just theatre.

For anyone interested in this space, I recommend Murray Shanahan’s paper [“Role Play with Large Language Models”](https://www.nature.com/articles/s41586-023-06647-8).

#### One piece of advice for folks wanting to get deeper into AI?

Kill the magic. Understanding how LLMs work reveals the power.

#### Who do you want to read a Tokens & Tactics interview from?

Dave and Pan from [Move37](https://www.move37.ai/) — absolute OGs of using generative AI for creative thinking.

---

If you have any questions, [please be in touch](https://brxnd.ai/contact).

Thanks for reading,

Noah and Claire