# Growing Minds — Child Development Study Hub

A buildless study companion based on eight supplied Child Development slide decks.

- 66 curated topics with examples, lecture timelines and 66 recall prompts.
- 80 single-best-answer MCQs, explanations, shuffled choices, pagination and missed-answer review.
- Searchable extracted text for 404 original slide sections and available embedded pictures.
- Browser-local bookmarks, study progress and answer history; responsive layout and dark theme.
- Correction notes distinguish selected outdated or misleading slide claims from curated study material.

## Run
Serve `dist/` with a static HTTP server. No package installation or build step is required.
Run `python build_content.py` from this directory to regenerate `dist/data.json` from the stored extraction and authored content. Check JavaScript with `node --check dist/app.js`.

## Source fidelity
Original text retains source wording; notes are adapted educational explanations. Available embedded pictures from seven decks are included. Native shape diagrams and original page layouts are not reproduced. Lecture 6 was recovered from a legacy PowerPoint binary: its text is included but image layout could not be recovered. Blank/title/reference pages remain in the original order. Source lecture files are credited in the website footer. Supporting primary resources are linked in the Resources view.

Milestones are approximate guides and this companion does not provide individual diagnoses. Historical statistics remain in the original source sections with context warnings.

## Put this repository on GitHub

1. Extract the ZIP and create an empty GitHub repository.
2. In GitHub Desktop, choose **File → Add local repository**, select the extracted folder, and choose **Create a repository here** if prompted. Commit the files and choose **Publish repository**. Keep it private unless you intend to share the supplied lecture material.
3. For GitHub Pages, open repository **Settings → Pages → Build and deployment → Source → GitHub Actions**. The included workflow publishes `dist/` when you push to `main`; you can also run it manually from Actions. Pages availability for private repositories depends on your GitHub plan. A Pages site may expose lecture material publicly; check the intended audience before enabling it.

### Command-line alternative

```bash
git init -b main
git add .
git commit -m "Initial child development study website"
```

Then connect the repository to your own GitHub remote and push `main`.

### Preview locally

```bash
python -m http.server 8000 --directory dist
```

Open http://localhost:8000 . Avoid opening index.html directly because the site loads its JSON with fetch.

No API keys, passwords, original Sites project configuration or Git remote credentials are included. This package contains source files rather than another account's Git history. Lecture text and embedded illustrations retain their source attribution; no rights to third-party course material are granted by this package.
