# Erin Barrett — personal portfolio

A static Jekyll site for the GitHub Pages user site `eebarr14.github.io`. The pages are written in Markdown with YAML front matter; shared structure and navigation live in Jekyll layouts and includes.

## Update the site

- Edit `index.md`, `about.md`, `work-experience.md`, or `contact.md` to update page content.
- Keep each page’s YAML front matter at the top of the file. The title, description, permalink, and layout fields are used by Jekyll and the SEO plugin.
- Update `_data/navigation.yml` to change the navigation labels or destinations.
- Update `assets/css/site.css` to change the visual design.
- The contact page intentionally has no public email address or `mailto:` link. Replace its placeholder only with a contact method you want to publish.
- Do not add unsupported facts or achievements; use information you have approved for public display.

## Preview locally

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`. To check the generated site without serving it:

```sh
bundle exec jekyll build
```

The site output is written to `_site/`.

## Publish with GitHub Pages

1. Use a GitHub repository named `eebarr14.github.io`.
2. Push the site source to the repository’s `main` branch.
3. In **Settings → Pages**, select **Deploy from a branch**, then choose `main` and the `/ (root)` folder.
4. GitHub Pages builds this Jekyll site automatically. No separate build workflow or manual build step is required.

The Jekyll configuration uses `url: "https://eebarr14.github.io"` and an empty `baseurl`, as required for a user site. Internal links use the `relative_url` filter.

## Run Lighthouse

With the local Jekyll server running, use a current Chrome/Chromium installation and Lighthouse:

```sh
npx --yes lighthouse http://127.0.0.1:4000 \
  --only-categories=performance,accessibility,best-practices,seo \
  --view
```

For a saved report instead of opening the viewer:

```sh
npx --yes lighthouse http://127.0.0.1:4000 \
  --only-categories=performance,accessibility,best-practices,seo \
  --output=html --output-path=./lighthouse-report.html
```

The report is a local test artifact; do not commit it unless you intend to publish it.

## Technical choices and assumptions

- The `github-pages` gem pins the site to GitHub Pages-compatible Jekyll plugins. `jekyll-seo-tag` supplies page metadata and `jekyll-sitemap` generates `/sitemap.xml`.
- The light/dark switch is a native checkbox styled with CSS; it has no JavaScript dependency and does not save a preference between page loads.
- The mountain illustration and favicon are local SVG files. The site does not load third-party fonts, images, scripts, or trackers.
- Your supplied résumé is the source for portfolio content. No email address, profile URL, portrait, clients, projects, or extra metrics were supplied, so they are omitted or marked as placeholders.
- The firm name “Paul, Weiss, Rifkind, Wharton & Garrison LLP” is spelled “Rifkind” here; the résumé text supplied “Rikfind.”