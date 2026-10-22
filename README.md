# Ibrahim Khalaf — Portfolio

Personal portfolio site for **Ibrahim Khalaf (Ibrheam)** — freelance developer from Gaza.

- Live: https://ibrheamkhalaf88-collab.github.io/portfolio/
- Repo: https://github.com/ibrheamkhalaf88-collab/portfolio

## Stack
Single-file static site: `index.html` (HTML + CSS + JS, no build step).
Hosted on GitHub Pages.

## How to edit

All content lives in 3 arrays near the bottom of `index.html`:
- `SKILLS` — grouped skill tags
- `PROJECTS` — name, idea (ar/en), tech, shot (image URL), link, github
- `SERVICES` — title, price, desc

### Add a new project
Append an object to `PROJECTS`:
```js
{
  name: "My Project",
  featured: false,
  idea: { ar: "...", en: "..." },
  tech: ["React", "Node"],
  shot: "https://opengraph.githubassets.com/1/OWNER/REPO",  // or any image URL
  link: "https://...",
  github: "https://github.com/..."
}
```

### Add a new page
Create a new `.html` file in this folder and link it from the nav in `index.html`.

### Change contact links
Edit the contact section in `index.html` (Telegram/WhatsApp placeholders).

### Change splash screen
Edit the `#splash` block + `splashInit()` in `index.html`. Set `SPLASH_ONCE = false` to show every visit.

## How to publish
```bash
git add .
git commit -m "update portfolio"
git push
```
GitHub Pages rebuilds automatically.

## Local preview
Just open `index.html` in a browser. No server needed.
