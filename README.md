# Shengxi Gui — personal academic website

This repository contains a Jekyll site for GitHub Pages, adapted from
[academic-homepage](https://github.com/luost26/academic-homepage).

## Update the content

- Profile, contact links, biography, education, and experience: `_data/profile.yml`
- Navigation: `_data/navigation.yml`
- Homepage display options and footer: `_data/display.yml`
- Publications: add or edit Markdown files in `_publications/<year>/`
- News: add or edit Markdown files in `_news/`
- Research directions, descriptions, figure paths, methods, and related
  publications: `_data/research.yml`
- Research page structure: `research.html`
- Colors, typography, spacing, and responsive styles: `assets/css/global.css`

To add a figure for a research direction, save the image under
`assets/images/research/`, then set that direction's `image` value in
`_data/research.yml`, for example:

```yaml
image: "/assets/images/research/forest-wildfire.jpg"
```

## Preview locally

Install Ruby and Bundler, then run:

```powershell
bundle install
bundle exec jekyll serve
```

Open the local URL shown by Jekyll. Restart the server whenever `_config.yml`
changes.

## Publish with GitHub Pages

This is a GitHub user site: the repository name is `HeavenswordG.github.io`
and `_config.yml` uses `baseurl: ""` so every page and asset resolves from the
domain root.

In the GitHub repository, open **Settings → Pages**, choose **Deploy from a
branch**, and publish the root of the `main` branch. The website URL is
`https://heavenswordg.github.io/`.

## Before publishing

Review the email address, dates, biography, and publication list for accuracy.
Replace the GitHub avatar with a local portrait by saving it under
`assets/images/photos/` and updating `portrait_url` in `_data/profile.yml`.
