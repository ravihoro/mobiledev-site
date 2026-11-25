# mobiledev website

The developer site for **mobiledev**, showing our Android apps: **Dotify**, **Cineframe**, and **Animate** (coming soon).

## What's here

A single static page, no build step:

| File | What it is |
|---|---|
| `index.html` | The whole page: HTML with its CSS inline |
| `img/dotify/` | Dotify icon, Galaxy face demo loop and poster, dot icons screenshot |
| `img/cineframe/` | Cineframe icon and 65:24 panoramic artwork |
| `img/animate/` | Animate icon, demo loop and poster |

Images are copied from `dotify-site`, `cineframe-site` and `animate-site`.

## Editing

Preview through a local server rather than by double-clicking the file:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## When Animate launches

In the `#animate` section of `index.html`, remove the two "Coming soon" badges and replace the `.btn-soon` span with a Google Play link (https://play.google.com/store/apps/details?id=com.animate_app.app), and drop the "Soon" tag from the hero pill.

## Deploying

Like the app sites, this deploys through Cloudflare Pages once the project is connected to a repository. Build settings: framework preset **None**, build command **empty**, output directory **`/`**.
