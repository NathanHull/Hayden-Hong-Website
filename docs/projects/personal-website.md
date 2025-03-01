---
sidebar_position: 1
description: The page you're looking at right now!
---

# Personal Website

:::info
[Check out the repo for this site on GitHub](https://github.com/AFRUITPIE/Hayden-Hong-Website).
:::

## Framework Choices

This is my third attempt at my personal website.

[The first attempt](https://github.com/AFRUITPIE/Hayden-Hong-React) was entirely in React, which made writing content difficult. It was hosted on AWS S3 and Cloudfront, which meant more maintenance than I wanted out of a weekend project.

[My second attempt](https://github.com/AFRUITPIE/Hayden-Hong-Blog-Jekyll) used [Jekyll](https://jekyllrb.com). Jekyll, being a [static site generator](https://en.wikipedia.org/wiki/Static_site_generator), made writing content a breeze. I found that Ruby dependencies were difficult to set up between machines.

### Obsidian Publish

[Obsidian Publish](https://obsidian.md/publish) was the first solution I looked into because [Obsidian](https://obsidian.md) is such a fantastic piece of software.

The feature set was perfect, but the price ($8/month at the time of writing) was impossible to justify for a personal webpage.

### Gatsby

[Gatsby](https://www.gatsbyjs.com) is highly recommended in a lot of threads on Hacker News. Unfortunately, I found Gatsby's docs to be hostile. Every conspicuous button on the Gatsby homepage links to a Netlify resource, Gatsby Cloud product page, or brand testimonial.

I'm sure Gatsby is a great framework, but I don't want to sift through ads every time I look at the docs.

### Docusaurus (The one I chose)

[Docusaurus](https://docusaurus.io) is what I ended up choosing for the third attempt because:

- It allows me to copy-paste the pages I had already written for Jekyll
- A large community uses it
- The docs are _excellent_
- It looks good out-of-the-box

## A note about light and dark color schemes

Webpages that don't support both a light and dark mode are just plain awful. Nobody likes opening a bright white page in the middle of the night and frying their eyes.

Some webpages have implemented an obnoxious toggle between light and dark mode, like _the Docusaurus docs:_

![Example of a dark and light more toggle](./assets/appearance-toggle.png)

**Stop doing this!** Just use [the `prefers-color-scheme` CSS Media Feature](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme) so my device can automatically tell you what color scheme to use.

[Docusaurus has an option to enable following `prefers-color-scheme`](https://docusaurus.io/docs/api/themes/configuration#color-mode---dark-mode), but disables it by default for some inexplicable reason.

## Hosting on Cloudflare Pages

My personal website is hosted in [Cloudflare Pages](https://pages.cloudflare.com). My reasoning is that Cloudflare is already my domain registrar, so integration with Cloudflare Pages is as easy as possible.

## Development Enviornment

I integrated my repo with [Dev Containers](https://containers.dev) and [GitHub Codespaces](https://github.com/features/codespaces), which brings me a reproducible environment across my dev machines.
