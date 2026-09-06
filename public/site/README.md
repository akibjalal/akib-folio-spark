# Akib Jalal — Portfolio (static site)

A single-page, fully static portfolio. No backend, no build step, no dependencies.
Open `index.html` in a browser and it works.

## Files

```
index.html                 All page content and sections
style.css                  Design system (colours, layout, responsive rules, animations)
script.js                  Theme toggle, mobile menu, scroll reveal, contact form
assets/images/             Profile photo and project screenshots
assets/icons/favicon.svg   Favicon placeholder
assets/resume/resume.pdf   Downloadable CV
```

## Deploying to GitHub Pages

1. Create a repository (e.g. `portfolio`) and upload the contents of this folder
   so that `index.html` sits at the repository root.
2. Repository → **Settings** → **Pages** → Source: *Deploy from a branch*,
   Branch: `main`, Folder: `/ (root)` → **Save**.
3. Your site goes live at `https://<username>.github.io/<repo>/`.

All asset paths are relative, so the site works from a repository subpath.

## How to update things later

| What | Where |
|---|---|
| Profile photo | replace `assets/images/profile.jpg` (square image works best — it is shown in a circle) |
| Resume PDF | Save it as `assets/resume/resume.pdf` — the button already points there |
| Social links | `index.html` → put the URL in `href` and delete `data-placeholder` |
| Skills | `index.html` → edit the four cards in the Skills section |
| Projects | the Projects section was removed while there is nothing to show — ask to add it back with real projects |
| Colours | `style.css` → the `:root` / `[data-theme="light"]` variables at the top |

## Notes

- Dark mode is the default; the toggle remembers the visitor's choice.
- The "Connect via Email" button opens the visitor's own email client (`mailto:`) —
  nothing is sent to a server, which keeps the site GitHub Pages compatible.
