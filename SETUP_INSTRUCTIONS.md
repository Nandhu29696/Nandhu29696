# Setup Instructions

## 1. Create your profile repo
Create a new **public** repository named **exactly** your GitHub username
(e.g. if your username is `nandhakumarm`, the repo must be named `nandhakumarm`).
GitHub auto-detects this special repo and shows its README on your profile page.

## 2. Replace the placeholder
Open `README.md` and replace every occurrence of `YOUR_GITHUB_USERNAME`
with your actual GitHub username (used in the snake animation, stats cards, and profile-view counter).

## 3. Add the README
Commit `README.md` to the root of that repo.

## 4. Enable the snake animation
1. In the same repo, create the folder path `.github/workflows/`
2. Add `snake.yml` (provided) into that folder.
3. Go to repo **Settings → Actions → General → Workflow permissions** and set it to
   **"Read and write permissions"** (required so the action can push the `output` branch).
4. Go to the **Actions** tab and manually run the "Generate Snake Animation" workflow once
   (don't wait for the daily cron) — this creates the `output` branch with the SVG.
5. The README already points to:
   `https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME/output/github-contribution-grid-snake-dark.svg`
   — once you've swapped in your username, it will render automatically.

## 5. Optional tweaks
- **Portfolio link**: the Portfolio badge currently links to `#` — swap in your real portfolio URL.
- **Stats theme**: currently `tokyonight` to match the dark/techy look — browse more themes at
  https://github.com/anuraghazra/github-readme-stats#themes
- **Typing text**: edit the `lines=` parameter in the typing SVG URL to change the animated headline text.

That's it — push to `main` and your profile page will show the full dark, animated README.
