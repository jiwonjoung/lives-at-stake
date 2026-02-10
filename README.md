# GitHub Pages deploy (animal lives chart)

This folder is a static site that fetches OWID API data in the browser, so it stays live even when your computer is off.

## What it does

- Uses OWID indicators directly at runtime (no local backend).
- Series: Poultry, Beef and buffalo, Sheep and goat, Pork.
- Includes `All countries` option, plus individual country selection.
- Includes `Sort by -> Total animals slaughtered` option.

## Quick publish (new repo)

1. Create a new GitHub repository, for example `animal-lives-chart`.
2. Copy this folder content (`index.html`) into the repo root.
3. Push to `main`.
4. In GitHub: `Settings -> Pages`.
5. Under `Build and deployment`, pick:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main` and `/ (root)`
6. Save, then wait 1-2 minutes.

Your site URL will be:

`https://<your-github-username>.github.io/<repo-name>/`

## Local preview

From this repo root:

```bash
.venv/bin/python -m http.server 8787 --directory ai/github-pages
```

Then open:

`http://127.0.0.1:8787`
