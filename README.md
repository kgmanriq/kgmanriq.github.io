# kgmanriq.github.io

Personal site for Katrina Manrique: resume + blog, built with Jekyll and hosted free on GitHub Pages.
Live at **https://kgmanriq.github.io**.

## Write a new blog post

1. Go to the `_posts` folder on GitHub and click **Add file → Create new file**.
2. Name it `YYYY-MM-DD-short-title.md` (e.g. `2026-11-05-lessons-from-statewide-rollouts.md`).
3. Start the file with:

   ```
   ---
   layout: post
   title: "Your post title"
   tags: [govtech, data]
   ---
   ```

4. Write the post below it in Markdown and click **Commit changes**. It's live in about a minute.

## Update the resume

- Text: edit `_data/resume.yml`. Every section of the resume page is pulled from there.
- PDF download: replace `assets/files/Katrina_Manrique_Resume.pdf` with a new file of the same name.

## Add a project

Add a file to `_projects` (e.g. `my-project.md`) starting with:

```
---
title: "Project name"
type: Publication        # small label shown on the tile
date: 2026-11-01         # newest projects show first on the home page
summary: One sentence shown on the tile.
tags: [AI governance]
---
```

Optional: `image: /assets/images/photo.jpg` adds a picture to the tile (works on blog posts too).

## Other things to edit

- Name, email, LinkedIn, sidebar links: `_config.yml`
- Home page overview and margin notes: `index.html`
- Colors and fonts: `assets/css/style.css` (the variables at the top)
- Any `## Heading` in a post or project automatically appears in the sidebar's "On This Page" list.

## Preview locally (optional)

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
