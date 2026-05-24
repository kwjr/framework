# Framework — The Works

**Project artifact tracking and governance tool** — part of The Works suite alongside Clockwork and Fieldwork.

## What it does

Framework helps you track the creation, rollout, and health of project governance artifacts across your entire portfolio. It supports 86 standard artifacts across 17 folders — from Initiation through Vendor & 3rd Party — and adapts the applicable artifact list based on each project's type (Conversions, Implementations, Agile, Consulting) and billing model (T&M, Fixed-Fee).

**Key features**
- Multi-project portfolio management
- Per-artifact status tracking with health scoring
- Portfolio dashboard with aggregate health metrics
- Per-project drill-down view with folder breakdown
- Cadence reference for all 86 artifacts
- Fully offline via service worker — works without internet after first load
- All data stored locally in your browser (nothing sent to any server)
- Installable as a PWA on desktop and mobile

## Deploying to GitHub Pages

1. **Fork or create a new repository** on GitHub
2. **Upload all four files** to the repository root:
   - `index.html`
   - `framework-sw.js`
   - `framework-manifest.json`
   - `.nojekyll`
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch` → `main` → `/ (root)`
5. Click **Save** — your site will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two

> **Tip:** After your first visit, Framework is fully cached for offline use. The service worker will keep the app available even without an internet connection.

## Installing as a PWA

Once deployed and opened in Chrome, Edge, or Safari:
- **Desktop (Chrome/Edge):** Click the install icon (⊕) in the address bar
- **iOS Safari:** Tap Share → Add to Home Screen
- **Android Chrome:** Tap the three-dot menu → Add to Home Screen

## Artifact status values

| Status | Health | Description |
|--------|--------|-------------|
| Not Started | 🟡 Attention | Default — work hasn't begun |
| In Progress | 🟡 Attention | Actively being worked |
| Complete | 🟢 Current | One-time artifact is done |
| Current | 🟢 Current | Recurring artifact is up to date |
| Stale | 🔴 Action Needed | Overdue for update — triggers action |
| N/A | 🟢 Current | Not applicable to this project |
| Deferred | 🟡 Attention | Intentionally postponed |
| Future | ⬜ Excluded | Belongs to a later project stage — not counted in health metrics |

## Data backup

Use **Settings → Download Backup** regularly to save a timestamped JSON file of all your projects. Restoring a backup also supports importing backups from the single-project v1 version of Framework.

## The Works suite

| Tool | Purpose | Status |
|------|---------|--------|
| Clockwork | Time tracking | Released |
| Fieldwork | Action item & to-do tracking | Released |
| Framework | Project artifact tracking | Released |
| Groundwork | Project planning | Planned |
| Legwork | Research & discovery tracking | Planned |
