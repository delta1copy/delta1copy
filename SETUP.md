# Setup & Troubleshooting Guide for `delta1copy`

This repository serves as the special profile README for **Sangaraju Charan Varma** (`delta1copy`).

---

## 🛠️ Editing Project Placeholders
- The `README.md` file contains project placeholders in the **Featured Projects** section.
- To update or replace placeholder project links, edit `README.md` directly on the `main` branch or submit a Pull Request.

---

## 🐍 Contribution Snake Workflow (`snake.yml`)
- The workflow located at `.github/workflows/snake.yml` generates the animated contribution grid snake SVGs:
  - `github-contribution-grid-snake.svg`
  - `github-contribution-grid-snake-dark.svg`
- It runs automatically on a scheduled cron (`0 0 * * *`), on pushes to `main`, or via manual trigger (`workflow_dispatch`).
- The generated SVG files are automatically pushed to the **`output`** branch of this repository.

---

## 🔍 Troubleshooting

### 1. GitHub Actions Permissions Error
- If the workflow fails to push to the `output` branch:
  1. Go to **Settings** > **Actions** > **General** in this repository.
  2. Scroll down to **Workflow permissions**.
  3. Select **Read and write permissions**.
  4. Save the changes and re-run the `Generate Contribution Snake` workflow.

### 2. External Widget Rate Limits / Images Not Loading
- Profile statistics cards (`github-readme-stats`, `github-readme-streak-stats`) rely on external API services.
- If they fail to display or show broken images, it is usually temporary due to rate limits or API downtime.
- The contribution snake images require the `output` branch to exist after the first workflow run.
