+++
date = '2026-03-02T19:38:29+08:00'
draft = false
title = 'Building This Blog: A Minimal Setup with Hugo & GitHub Pages'
description = 'How I set up a clean, fast, and free personal blog using Hugo, PaperMod, and GitHub Actions — from zero to deployment in 10 minutes.'
tags = ['Hugo', 'GitHub Pages', 'DevOps', 'Tooling']
categories = ['Engineering']
ShowToc = true
TocOpen = true
+++

## Why Build a Personal Blog?

Every engineer should have a corner of the internet they own. Not a Medium post buried in paywalls, not a tweet lost in the feed — a **real site**, under your name, that you control.

This blog is that for me. Here's exactly how I built it.

## The Stack

| Layer | Tool | Why |
|-------|------|-----|
| Generator | [Hugo](https://gohugo.io/) | Fastest static site generator. Sub-second builds. |
| Theme | [PaperMod](https://github.com/adityatelange/hugo-PaperMod) | Clean, minimal, dark mode, great typography. |
| Hosting | GitHub Pages | Free, reliable, HTTPS out of the box. |
| CI/CD | GitHub Actions | Auto-deploy on every push to `main`. |

> No databases. No servers. No monthly bills. Just Markdown files and `git push`.

## Setup in 5 Commands

```bash
hugo new site my-blog && cd my-blog && git init

git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod

hugo new posts/hello-world.md

hugo server -D
```

That's it. Write in Markdown, push to GitHub, deployed in seconds.

## The Deployment Pipeline

The entire CI/CD is a single GitHub Actions workflow:

1. **Push to `main`** triggers the pipeline
2. Hugo builds the site with `--gc --minify`
3. Output is uploaded as a GitHub Pages artifact
4. GitHub deploys it to the live URL

No Docker, no Vercel, no Netlify config — just native GitHub infrastructure.

## What's Next

- Deep dives into systems I'm building
- Architecture decisions and trade-offs
- Tools and workflows that make me faster

Stay tuned.
