# romeshprasad.github.io

Personal academic website of Romesh Prasad, built with Jekyll and hosted on GitHub Pages.

## Where to edit things

| What                                  | File                         |
|---------------------------------------|------------------------------|
| Name, title, email, profile links     | `_config.yml`                |
| Profile photo                         | `assets/img/profile.jpg` + `photo:` in `_config.yml` |
| Home page (about, stats, contact)     | `index.html`                 |
| Home page highlights                  | `_data/highlights.yml`       |
| Vision page                           | `vision.md`                  |
| Four research directions              | `_data/research.yml`         |
| Testbeds / other research             | `research.html`              |
| Publications                          | `_data/publications.yml`     |
| Teaching                              | `teaching.md`                |
| CV page / CV PDF                      | `cv.html` / `assets/files/Romesh_Prasad_CV.pdf` |
| Colors & fonts                        | `assets/css/style.css` (top) |

`romesh_documents/` holds private source documents and is git-ignored, so it is never published.

## Publishing changes

```bash
git add .
git commit -m "Describe the change"
git push
```

GitHub Pages rebuilds the site about a minute after each push.
