# [Lab Name] Website

A Jekyll site for the [Lab Name] at the University of Rhode Island, hosted on GitHub Pages.

## Where to edit things

| What                       | File                         |
|----------------------------|------------------------------|
| Lab name, PI, email, links | `_config.yml`                |
| Home page "About" text     | `index.md`                   |
| Research areas             | `_data/research.yml`         |
| Lab members                | `_data/people.yml`           |
| Publications               | `_data/publications.yml`     |
| News items                 | `_data/news.yml`             |
| Openings / how to apply    | `join.md`                    |
| Colors & fonts             | `assets/css/style.css` (top) |
| Logo                       | `assets/img/logo.svg`        |
| Member photos              | `assets/img/people/`         |

Search for `[` to find every placeholder that still needs filling in.

## Publish on GitHub Pages

1. Create a new public repository on GitHub.
   - Name it `<your-username>.github.io` for a site at `https://<your-username>.github.io`, **or**
   - give it any name (e.g. `lab`) for a site at `https://<your-username>.github.io/lab`.
     In that case, set `baseurl: "/lab"` in `_config.yml`.
2. Set `url:` in `_config.yml` to `https://<your-username>.github.io`.
3. Upload these files (drag and drop on GitHub works, or use git):
   ```bash
   git init
   git add .
   git commit -m "Initial lab website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo>.git
   git push -u origin main
   ```
4. On GitHub, open **Settings → Pages**, set **Source** to *Deploy from a branch*, then choose `main` / `(root)`.
5. Wait 1–2 minutes and the site will be live.

Tip: you can create a GitHub **organization** for the lab (e.g. `prasad-lab`) and name the repo
`prasad-lab.github.io`. That way the URL belongs to the lab, not to one person.

## Preview locally (optional)

Install Ruby (on Windows, use https://rubyinstaller.org, "with Devkit"), then:

```bash
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000.
