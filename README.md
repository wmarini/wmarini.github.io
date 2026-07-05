# wmarini.github.io

Personal blog. Jekyll on GitHub Pages — no local build required; GitHub
renders the site on every push to `main`.

Layout inspired by [journal.stuffwithstuff.com](https://journal.stuffwithstuff.com)
([munificent/journal](https://github.com/munificent/journal)).

## Adding a post

Create a markdown file in `_posts/` named `YYYY-MM-DD-slug.md`:

    ---
    title: "Debugging the debugger"
    categories: [gdb, nonstop]
    ---

    Post body in GitHub-flavored markdown. Fenced code blocks get
    syntax highlighting via Rouge: ```cpp, ```c, ```sh, ```rust, ...

Commit and push. The post appears at `/YYYY/MM/DD/slug/`, in the **by date**
tab under its year, and in the **by category** tab under each category listed
in the front matter. New categories need no registration — they appear
automatically.

## Structure

    _config.yml          site settings, permalink style, plugins
    _layouts/
      default.html       header / footer shell
      post.html          post page (date, categories, prev/next)
    _includes/
      post_row.html      one row in a post list (shared by both tabs)
    index.html           home page with "by date" / "by category" tabs
    about.md             about page (/about/)
    assets/css/style.css all styling (colors are CSS variables in :root)
    _posts/              one markdown file per post

## Tweaking the theme

All colors live in the `:root` block at the top of `assets/css/style.css`
(`--bg`, `--green`, `--text`, ...). Fonts are IBM Plex Mono (chrome, dates,
code) and Source Serif 4 (body), loaded from Google Fonts in
`_layouts/default.html`.

## Local preview (optional)

    gem install bundler
    bundle install
    bundle exec jekyll serve   # http://127.0.0.1:4000

## Housekeeping

The `_posts/2026-*-sample-*.md` files and `2026-07-03-style-test.md` are
placeholders — delete them once real posts exist.
