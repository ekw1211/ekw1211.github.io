# Personal Academic Page

A minimal academic personal website for GitHub Pages.

## File structure

```
index.html                    ← single-page app
posts/
  on-research-taste.md        ← blog posts (one file each)
  writing-clearly.md
projects/
  semantic-search.md          ← project detail pages
  citation-network.md
publications/
  publications.md             ← full publications list
```

## Setup on GitHub Pages

1. Create a repo named `yourusername.github.io`
2. Copy all files into the repo root
3. Push — GitHub Pages will serve `index.html` automatically

No build step, no dependencies to install.

## Adding content

### New blog post
1. Create `posts/my-new-post.md` with a frontmatter header:
   ```
   ---
   title: My Post Title
   date: 2025-01-15
   description: One-sentence summary shown in the list.
   ---

   Your content here…
   ```
2. Add an entry to the `POSTS` array near the top of `index.html`:
   ```js
   {
     file: 'posts/my-new-post.md',
     title: 'My Post Title',
     date: '2025-01-15',
     desc: 'One-sentence summary shown in the list.',
   },
   ```

### New project
1. Create `projects/my-project.md`
2. Add an entry to the `PROJECTS` array in `index.html`

### Publications
Edit `publications/publications.md` directly — it's plain markdown.

## Personalizing

Edit these things in `index.html`:

- **Name, affiliation, contact** — in the `<aside class="sidebar">` block and the About section
- **External links** — the `.sidebar-links` block (email, GitHub, Scholar, CV)
- **About text** — the `#about` section body

Colors and fonts are defined as CSS variables at the top of the `<style>` block.
