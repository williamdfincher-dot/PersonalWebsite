# willfincher.com

My personal site. It's a [Jekyll](https://jekyllrb.com) site that GitHub Pages
builds automatically every time something is pushed to `main`. There's nothing
to install or deploy.

## Writing a blog post

1. Create a file in the `_posts/` folder named `YYYY-MM-DD-post-title.md`,
   for example `_posts/2026-11-05-why-i-started-writing.md`.
   (On GitHub: open `_posts/`, then **Add file → Create new file**.)
2. Start it with this header, then write the post in Markdown below it:

   ```markdown
   ---
   title: "Why I Started Writing"
   description: "Optional. One sentence used for link previews."
   ---

   Post text goes here.
   ```

3. Commit to `main`. The post appears at `willfincher.com/blog/post-title/`
   within a minute or two, and it's added to the blog page, the home page and
   the RSS feed.

`_drafts/example-post.md` is a template with a Markdown cheat sheet. Anything in
`_drafts/` is never published, so it's a good place for works in progress.

**Images:** upload them to `assets/images/` and use
`![description](/assets/images/file.jpg)` in the post.

**Editing or removing a post:** edit or delete its file in `_posts/`.

## Editing the rest of the site

| What | File |
|---|---|
| Home page intro | `index.html` |
| About page | `about.md` |
| Projects list | `_data/projects.yml` |
| Nav links, site title | `_config.yml` |
| Colors and fonts | `assets/css/style.css` (colors are at the top) |

## Previewing locally (optional)

```bash
gem install jekyll jekyll-feed jekyll-seo-tag
jekyll serve
```

Then open http://localhost:4000.
