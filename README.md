# The Inner Light — Landing Page

A single-page website for **The Inner Light: Learning to Begin Again**, a book on spirituality, positive psychology, and healing by **Ashwik Bire**.

🔗 **Live site:** `https://ashwikbire.github.io/The-Inner-Light/` *(update this once you know your actual repo name — see [Setup](#setup) below)*
📖 **Get the book:** [Amazon Kindle](https://amzn.in/d/04r3G7PS)

---

## What's in this repo

| File | Purpose |
|---|---|
| `index.html` | The entire site — hero, about, chapter highlights, author bio, buy links. Self-contained (HTML/CSS/JS in one file). |
| `cover.jpg` | Book cover image, used as the social-share preview (Open Graph / Twitter Card). **Must stay in the repo root alongside `index.html`** — the page references it by relative path. |
| `README.md` | This file. |

No build step, no dependencies, no framework — just static files. Fonts (Playfair Display, EB Garamond) load from Google Fonts via CDN at runtime.

---

## Setup

1. Create a new GitHub repository (or use an existing one).
2. Upload **both** `index.html` and `cover.jpg` to the repository root.
3. Go to **Settings → Pages**.
4. Under **Source**, select the branch (usually `main`) and folder `/ (root)`.
5. Save. GitHub will publish the site at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```
6. It can take a minute or two for the first deploy to go live.

If you want this to be your primary GitHub Pages site (`ashwikbire.github.io` with no sub-path), name the repository exactly `ashwikbire.github.io` instead, and it will be served from the domain root.

---

## Local preview

No server required — just open the file directly:

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or, for a closer-to-production preview (recommended, since some browsers restrict local file access):

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## Updating content

- **Buy link:** search `index.html` for `amzn.in/d/04r3G7PS` — it appears in a few places (hero button, closing CTA, nav bar, meta tags). Replace all instances if the link ever changes.
- **Cover image:** swap `cover.jpg` with a new file of the same name, or update the `<img>` `src` and the `og:image` / `twitter:image` meta tags if you rename it.
- **Author links:** LinkedIn, portfolio, and other links live in the "About the Author" section and the footer.

---

## About the book

*The Inner Light* moves between two traditions rarely given equal weight: positive psychology's evidence-based understanding of what helps people thrive, and spirituality's older, slower vocabulary for meaning, pain, and awareness. Across an introduction, fifteen chapters, and a closing reflection, it explores identity, inner pain, letting go, forgiveness, gratitude, purpose, and compassion — closing with a simple daily practice readers can return to.

## About the author

**Ashwik Bire** is a data scientist, researcher, and author based in Pune, Maharashtra, India. In May 2025, a posterior circulation stroke led to a recovery process that combined medical treatment with self-directed research into neuroscience, positive psychology, and neuroplasticity — the lived experience this book draws from.

- [LinkedIn](https://linkedin.com/in/ashwik-bire-b2a000186)
- [Portfolio](https://ashwikbire.github.io/My-Portfolio/)
- [The Human Mind](https://ashwikbire.github.io/The-Human-Mind/)

---

## License

The site's code (HTML/CSS/JS) is free to reuse or adapt. The book's text, cover artwork, and illustrations are © 2026 Ashwik Bire — all rights reserved.
