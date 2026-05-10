# Studio Arts – GitHub Pages Jekyll Site

A simple Jekyll site for an art teacher featuring Classes, Gallery, About, and Contact pages.

## Local Setup

1. Ensure you have Ruby (>= 3 recommended). A `.ruby-version` file is included (3.2.2). With a version manager (rbenv/asdf/rvm) run `rbenv install 3.2.2` or equivalent if needed.
2. Install dependencies:

```
bundle install
```

3. Run the local server:

```
bundle exec jekyll serve
```

4. Visit http://localhost:4000

## Deploying to GitHub Pages

If this repository name is `username.github.io` it will deploy automatically from the default branch.
If it's a project site, enable GitHub Pages in repo settings and set:

In `_config.yml` set:

```
url: "https://your-username.github.io"
baseurl: "" # or "/repo-name" for project site
```

Commit & push. GitHub Pages with `github-pages` gem will build the site.

## Content Management

- Classes are stored as collection items in `_classes/`. Add new markdown files with front matter.
- Gallery images: place assets in `assets/images/` and list them in `_data/gallery.yml`.
- Navigation is defined in `_config.yml` under `nav:`.

## Adding a New Class

Create a file like `_classes/figurative-painting.md`:

```
---
title: Figurative Painting
level: Intermediate
age_range: Adults
schedule: Mondays 18:00–20:00
fee: $240 (6 weeks)
---
Focus on gesture, proportion, and expressive color while working from life and reference.
```

## Forms

Contact form uses Formspree. Replace `your-form-id` in `contact.md` with a real endpoint.

## License

You may adapt and use this site freely.
