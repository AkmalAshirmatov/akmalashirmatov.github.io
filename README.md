# akmalashirmatov.github.io

Personal academic homepage of Akmal Ashirmatov, built on the
[Minimal Light](https://github.com/yaoyao-liu/minimal-light) Jekyll theme (CC0) and hosted with GitHub Pages.

## Where to edit

| What | File |
| --- | --- |
| Name, position, email, sidebar links, font, dark mode | `_config.yml` |
| About Me, News, Experience, Projects, Awards | `index.md` |
| Publications (title, authors, venue, buttons, badges, teaser) | `_data/publications.yml` |
| Publication entry markup | `_includes/publications.md` |
| Extra styles (badges, entry lists, mobile) | `assets/css/custom.css`, `assets/css/custom-dark.css` |
| Profile photo, favicon | `assets/img/avatar.jpg`, `assets/img/favicon-blank.svg` |
| Paper teaser figures | `assets/img/papers/` |
| CV | `assets/files/Akmal_Ashirmatov_CV.pdf` |

To add a paper, copy one block in `_data/publications.yml` and put its teaser figure in `assets/img/papers/`.
Wrap your own name in `<strong>…</strong>` so it is highlighted in the author list.

## Deploy with GitHub Pages

1. Create a public repository named **`AkmalAshirmatov.github.io`** on GitHub.
2. Push this folder to its `main` branch:
   ```bash
   git remote add origin https://github.com/AkmalAshirmatov/AkmalAshirmatov.github.io.git
   git push -u origin main
   ```
3. In the repository, open **Settings → Pages** and set **Source: Deploy from a branch**, branch **`main`**, folder **`/ (root)`**.
4. After a minute or two the site is live at <https://akmalashirmatov.github.io/>.

## Preview locally (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```
