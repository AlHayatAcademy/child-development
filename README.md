# Growing Minds — Child Development

Complete website for eight Child Development lectures. `index.html` is in the repository root. No build tools, dependencies or API keys are required.

## Update your GitHub repository

1. Extract this ZIP.
2. Copy the CONTENTS of `Child_Development_Full_Repo` into your existing `child-development` repository folder. Replace matching files. Keep your existing `.git` folder.
3. Verify that index.html, style.css, app.js, data.json and assets/ are directly in the repository root, not inside a nested folder.
4. Commit and push with GitHub Desktop.
5. Under Settings → Pages, choose Deploy from a branch, select main and / (root), and save. If your default branch differs, select that branch.
6. Wait for deployment, then refresh using Ctrl + F5.

No GitHub Actions workflow is required. The previous dist/ directory is unused with this layout.

## Local preview

Run `python -m http.server 8000` here and open http://localhost:8000 . An HTTP server is required because the site uses fetch to load JSON.

## Contents

Eight lectures; 66 topics with examples and timelines; 80 MCQs with explanations; 66 recall prompts; 404 source slide sections with available embedded pictures; assignments and supporting resources. Includes search, bookmarks, browser-local progress, missed-answer review, shuffled options, 10/20/50/100 question pagination, responsive layout and dark mode.

## Maintenance

Edit build_content.py and run `python build_content.py` to regenerate data.json. Original extracted text is in source-material/slides.json. Check JavaScript using `node --check app.js`.

## Source fidelity

The Source slides view preserves original wording, including dated estimates and spelling errors. Curated notes clarify selected misleading claims. Original attribution appears in the footer. Available pictures from seven decks are included. Native shape diagrams and original slide layouts are not reproduced. Lecture 6 text was recovered from a legacy file, but its picture layout was unavailable. Original PowerPoint binaries are not included.

Milestones are approximate guides, not individual diagnoses. Source material retains its original attribution; this package grants no rights to third-party course material. No credentials, Git history or account-specific hosting configuration is included.
