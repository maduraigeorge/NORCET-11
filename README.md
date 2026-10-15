# NORCET-11 Placement Desk (GitHub Pages)

Static copy of the dashboard. It reads two CSV files in `data/` and re-checks them every 30 seconds.

## Publish

1. On github.com create a new repository, for example `norcet11-dashboard`. Do not reuse `operations`.
2. In this folder run:

```
git init
git add .
git commit -m "NORCET-11 dashboard"
git branch -M main
git remote add origin https://github.com/<your-user>/norcet11-dashboard.git
git push -u origin main
```

3. On GitHub open Settings, then Pages. Set Source to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After about a minute the page is at `https://<your-user>.github.io/norcet11-dashboard/`.

## Update the data

Replace the files in `data/` (keep the column names), then commit and push. Open pages pick up the change after GitHub Pages redeploys and its cache expires, usually within a few minutes.

## Privacy

GitHub Pages on a free account needs a public repository. The CSVs hold roll numbers, categories, genders, scores and ranks from the public AIIMS result notice. Publish only if that is acceptable.
