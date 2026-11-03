# Czak Research Group website

Group site for the Czak Research Group (Department of Physics & Astronomy, James Madison University), built on the same AcademicPages/Jekyll theme as https://jasonczak.github.io/.

## Deploy

1. Create a repository named `CzakResearchGroup` under the JasonCzak account and push these files to the `main` branch.
2. In **Settings → Pages**, set **Source** to **GitHub Actions**. The included workflow (`.github/workflows/jekyll.yml`) builds and deploys on every push.
3. The site appears at https://jasonczak.github.io/CzakResearchGroup/

To host it elsewhere (for example a `czakresearchgroup.github.io` organization repo), change `url` and `baseurl` in `_config.yml`.

## Where things live

- Pages: `_pages/` (about.md is the home page)
- Menu: `_data/navigation.yml`
- Publications: `_publications/` (one file per paper; `category: manuscripts` or `inprep`)
- Presentations: `_talks/`
- Photos: `images/group/`; simulation videos: `assets/videos/`
- Downloadable files (outreach slides): `files/`
- Extra styles (videos, photo grids): `_sass/layout/_group.scss`
