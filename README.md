# Personal Website — Smitom Swapna Borah

This is the source repository for [smitomborah.com](https://smitomborah.com), a personal academic portfolio website built with [Hugo](https://gohugo.io/) using the [Anatole theme](https://github.com/lxndrblz/anatole) and deployed automatically via [Netlify](https://netlify.com).

---

## How it works

Every time a commit is pushed to the `master` branch, Netlify automatically rebuilds and redeploys the website. You do **not** need to run Hugo locally — just edit the files and push.

---

## Repository structure

```
.
├── assets/
│   └── source_files/        # Source files (e.g., PowerPoint diagrams) for reference
├── config/_default/
│   ├── params.toml          # Site-wide settings: name, profile picture, social links, etc.
│   ├── menus.en.toml        # Navigation menu items and their URLs
│   └── languages.toml       # Language settings
├── content/english/         # All page content (edit these to update the website)
│   ├── about_me.md          # About Me page
│   ├── research.md          # Research page
│   ├── publications.md      # Publications page
│   ├── news.md              # News page
│   └── contact.md           # Contact page
├── static/
│   └── images/              # Images used on the site
├── netlify.toml             # Netlify build configuration and redirects
└── themes/anatole/          # Hugo theme (do not edit)
```

---

## How to manually edit the website

### Editing page content

All pages live in `content/english/`. Each file is a Markdown (`.md`) file with a front matter block at the top (between the `---` lines) followed by the page content.

**Example — updating your About Me:**
1. Open `content/english/about_me.md`
2. Edit the text below the second `---`
3. Commit and push to `master`

Markdown basics:
- `**bold**` → **bold**
- `*italic*` → *italic*
- `[link text](https://url.com)` → hyperlink
- `## Heading` → section heading
- `---` → horizontal divider

### Adding or replacing an image

1. Place the image file in `static/images/`
2. Reference it in a content file as `/images/your-image.png`
3. To embed with a caption, use: `{{< figure src="/images/your-image.png" caption="Your caption" width="100%" >}}`

### Updating site-wide settings

Edit `config/_default/params.toml` to change:
- Your name and profile description (shown in the sidebar)
- Profile picture (`profilePicture`)
- Social media links

### Updating the navigation menu

Edit `config/_default/menus.en.toml` to add, remove, or reorder menu items.

### Changing the color scheme

In `config/_default/params.toml`, set `displayMode` to control the site theme:
- `"light"` — white background (current)
- `"dark"` — dark background
- `"auto"` — follows the visitor's system preference

### Updating the CV link

In `content/english/about_me.md`, find the line:
```
Here is my [CV](https://drive.google.com/...)
```
Replace the Google Drive URL with the new link.

---

## Source files

Editable source files for figures and diagrams are stored in `assets/source_files/`:

| File | Description |
|---|---|
| `Research_ConceptualDiagram.pptx` | PowerPoint source for the research interests conceptual diagram (Figure 1 on the About Me page) |

To update the figure on the website:
1. Edit the PowerPoint in `assets/source_files/Research_ConceptualDiagram.pptx`
2. Export the slide as a PNG
3. Replace `static/images/research_interests_figure.png` with the new export
4. Commit and push

---

## Deployment

- **Live site:** [smitomborah.com](https://smitomborah.com)
- **Hosting:** Netlify (auto-deploys on push to `master`)
- **Hugo version:** 0.120.4
