# think lab website

Plain Jekyll site, no theme or plugins.

- Pages: `index.md` (about), `position/`, `people/`, `news/`. `projects/` and `publications/` are ready but hidden: remove them from `exclude` in `_config.yml` and add them back to `_includes/nav.html`.
- People: `_data/people.yml` (photos in `assets/img/`)
- Projects: one file per project in `_projects/`
- News: one file per item in `_news/`
- Publications: `_data/publications.yml`
- Styles: `assets/css/site.css` (type scale 14 / 17 / 22 / 30, Lexend)

Local preview: `bundle install && bundle exec jekyll serve`
