# Zewei Zhang Academic Homepage

This repository contains the static personal academic website for Zewei Zhang, based on the Luka Homepage Template. It is designed for GitHub Pages and uses only plain HTML, CSS, and a small JavaScript file.

No React, Next.js, Hugo, Jekyll, npm, or build system is required.

## Editing The Site

Most content lives in `index.html`. The file has HTML comments around the main editable sections:

- Hero / profile sidebar
- About Me
- News
- Research Interests
- Selected Research
- Education
- Experience / Teaching / Awards
- Contact

For research entries, edit the cards inside the `Selected Research` section. Each card supports category tags, a figure, title, summary, authors, venue/status, role, and links such as Paper, Code, Project Page, Dataset, Slides, Poster, or Blog.

Keep unknown public links inside HTML comments or leave them out of the public page until the links are real. Do not add private contact details.

## Asset Locations

- CV: replace `assets/files/cv.pdf`
- Avatar: replace `assets/img/avatar.png`
- Institution logo: replace `assets/img/institution.svg`
- Favicon: replace `assets/img/favicon.svg`
- Project images: add files under `assets/img/projects/`; current card figures are `trajloom-card.png`, `imitsat-card.png`, and `gooddrag-card.jpg`
- Slides: add files under `assets/files/slides/`
- Posters: add files under `assets/files/posters/`

The institution logo and favicon are placeholders.

## Preview Locally

From the repository folder:

```powershell
cd "C:\F\文件\new personal\personal_web"
py -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

If `py` is unavailable, use:

```powershell
python -m http.server 8000
```

## Publish With GitHub Pages

Create the target repository:

```text
<MY_GITHUB_USERNAME>/<MY_GITHUB_USERNAME>.github.io
```

Then connect and push:

```powershell
git add .
git commit -m "Finalize academic homepage"
git remote add origin https://github.com/<MY_GITHUB_USERNAME>/<MY_GITHUB_USERNAME>.github.io.git
git push -u origin main
```

In GitHub, open repository settings and configure Pages:

- Source: Deploy from a branch
- Branch: `main`
- Folder: `/ root`

Do not create `CNAME` unless a custom domain is ready. Add one later only after DNS is configured.

## Future Update Checklist

- Verify that Google Scholar and LinkedIn point to your preferred public profiles.
- Add ORCID only if you want to publish a real ORCID URL.
- Replace or add paper, code, dataset, slides, and poster links only after they are public.
- Replace the placeholder institution logo.
- Update News with dated items and keep only 3-5 compact entries.
- Check `assets/files/cv.pdf` before publishing a new CV.
- Before every public commit, confirm the repository does not include private contact details, private addresses, unpublished confidential material, or other sensitive personal information.

## Attribution

This site is based on the [Luka Homepage Template](https://github.com/wzsyyh/luka-homepage-template) by Yuheng Yang.
