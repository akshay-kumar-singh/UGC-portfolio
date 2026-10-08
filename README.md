# Technical explainer videos

The one-page portfolio I send to brands: four explainer videos from my own channels
(After You Tap and Before You Merge) with links to where they're posted, the channels
themselves, what a client gets, and rates.

**Live:** https://akshay-explains.netlify.app

## Changing it

Edit, commit, push. Netlify publishes every push to `main` within a minute. There is
nothing to build; the site is these files as they are.

- **A new video:** add `videos/<name>.mp4` and a 540×960 `posters/<name>.jpg`, then
  copy one `<article class="reel" id="<name>">` block in `index.html`. The `id` is the
  link that opens that video directly: `akshay-explains.netlify.app/#<name>`.
- **The outreach reads this page.** Each video's `id`, title, first line and tag are
  what the dashboard pitches to brands, so keep that shape when you add one. Old links
  (`#duplicate-payments` and the other first samples) open the closest new video.
- **The link preview** shown in LinkedIn, WhatsApp and email is `og.jpg` (1200×630).
- **Light and dark:** the page follows the visitor's device; the button at the top
  right switches it and remembers the choice.
