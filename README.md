# joe-iervolino.github.io

My personal portfolio, showcasing my projects and interests.

Built with [Astro](https://astro.build) + [Tailwind CSS](https://tailwindcss.com),
based on the [devportfolio](https://github.com/RyanFitzgerald/devportfolio) template.

## Status

Scaffolded with lorem-ipsum placeholder copy. All content lives in a single file —
edit [`src/config.ts`](src/config.ts) to fill in the real name, title, about text,
skills, projects, experience, and education. No component edits needed for content.

## Local development

```bash
npm install
npm run dev
```

Then open http://localhost:4321.

| Command           | Action                                    |
| ----------------- | ----------------------------------------- |
| `npm install`     | Install dependencies                      |
| `npm run dev`     | Start the dev server at `localhost:4321`  |
| `npm run build`   | Build the production site to `./dist`     |
| `npm run preview` | Preview the production build locally      |

## Deployment

`.github/workflows/deploy.yml` builds the site and publishes it to GitHub Pages on
every push to `main`.

One-time setup: in the repo's **Settings → Pages**, set **Source** to
**GitHub Actions**.

## Structure

```
src/
  config.ts              # all site content lives here
  pages/index.astro      # page shell, section order
  components/            # Header, Hero, About, Projects, Experience, Education, Footer
  styles/global.css      # Tailwind entry + global styles
public/favicon.svg
```

Sections render conditionally — empty out an array in `config.ts` and that section
(plus its nav link) disappears.
