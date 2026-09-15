# GitHub Profile Upgrade — Setup

This package contains:

- `README.md` — redesigned profile README
- `.github/workflows/pacman.yml` — Pac-Man contribution animation
- `.github/workflows/metrics.yml` — analytics + isometric contribution calendar

## 1. Replace your current profile README

Copy `README.md` into your profile repository:

`i-shashikant/i-shashikant/README.md`

## 2. Enable Pac-Man

1. Push `.github/workflows/pacman.yml`.
2. Open **Actions**.
3. Select **Update Pac-Man Contribution Graph**.
4. Click **Run workflow**.
5. Wait for it to finish.
6. An `output` branch should appear.

The workflow also refreshes the animation daily.

## 3. Enable the metrics / isometric calendar

The metrics workflow needs a GitHub Personal Access Token stored as:

**Settings → Secrets and variables → Actions → New repository secret**

Secret name:

`METRICS_TOKEN`

Do not put the token directly in the README or workflow.

Then run:

**Actions → GitHub Metrics → Run workflow**

The workflow will create/update:

`github-metrics.svg`

The README already references that file.

## 4. Why some cards are external

GitHub Readme Stats, Streak Stats, the Activity Graph and Profile Trophy are dynamic third-party services. They are convenient, but any public shared service can occasionally experience caching, rate limits or downtime.

The important data remains on GitHub itself; the cards are presentation layers.

For maximum reliability later, we can self-host the stats cards too.

## 5. Included features

- Profile views
- Followers
- Public repository count
- Portfolio/contact buttons
- About section
- Featured projects
- Tech stack
- GitHub statistics
- Top languages
- Contribution streak
- Recent activity graph
- GitHub trophies
- Isometric contribution calendar
- Pac-Man contribution animation
- Experience
- Learning section
- Social links
