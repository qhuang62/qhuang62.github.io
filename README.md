# qhuang62.github.io

Personal academic site. Plain HTML + one stylesheet, no build step, no Jekyll
(`.nojekyll` is present).

```
index.html   the whole page
style.css    the whole stylesheet
pics/        profile photo, research figures, footer photo strip
cv/          CV_QinHuang.pdf
```

## Deploy

```bash
git init && git add -A && git commit -m "Initial site"
gh repo create qhuang62.github.io --public --source=. --push
```

GitHub Pages serves a `<user>.github.io` repo from the default branch root
automatically. Live at https://qhuang62.github.io within a minute or two.

To preview locally: `python3 -m http.server 8777` then open http://127.0.0.1:8777

## Theme

Follows the visitor's OS light/dark setting (which auto-switches at their real sunset
on macOS/iOS/Windows). A toggle in the nav overrides it; the choice persists in
`localStorage` under key `theme`. An inline script in `<head>` applies it before first
paint so there's no flash of the wrong palette.

## Still to fill in

Every item below is marked with a `TODO` comment in `index.html`.

- [ ] **CV** — add `cv/CV_QinHuang.pdf`. Two links point at it (hero + News footnote).
- [ ] **ORCID** — the hero ORCID link is a bare `https://orcid.org/`.
- [ ] **Analytics** — sign up free at https://www.goatcounter.com, pick a code, then
      replace `MYCODE` in the two commented blocks (script near `</body>`, Stats link in
      the footer) and uncomment both. No cookies, no consent banner.
- [ ] **Footer links** — four `href="#"` placeholders: Aquanauts at ASU, film photography
      site, ASU Search profile, Columbia Water Center people page.
- [ ] **Photo strip** — six images at `pics/strip-1.jpg` … `strip-6.jpg`, then uncomment the
      `PHOTO STRIP` block near the bottom of `index.html`.
- [ ] **Research figures** — three commented-out `<img class="fig">` tags in the Research
      section (`pics/wjj.png`, `pics/tc.png`, `pics/fire.png`).
- [ ] **EGU 2026 exact dates** — currently "April–May"; the two EGU entries and the News item.

## Publication list provenance

Built from Google Scholar (`user=5OZSGR0AAAAJ`, sorted by date) cross-checked against the
DOIs in your tracker. Two things worth a second look:

- Scholar listed *Targeted adaptive chaos control of regimes and eddy strength in two Lorenz
  models* under both **EGUsphere (2025)** and **Chaos, Solitons & Fractals (2026)**. It is
  listed here once, as the journal version. Confirm there isn't a separate preprint to cite.
- Author order was taken from Scholar. Worth one pass to confirm, especially the
  co-first-author asterisks on the MS8 talk (Huang* / Liu*), which the site does not currently
  mark.

## Press

Deliberately limited to major and official outlets: The Weather Channel, Gizmodo, Les Échos,
Phys.org, ASU News, EurekAlert!/AAAS, and UNDRR PreventionWeb. Left off on purpose: Daily Mail
(tabloid), and Scienmag / Earth.com / Scimex / South Florida Reporter (press-release
aggregators). Still pending per your tracker and not yet listed: CBC (Torah Kachur) and USA
Today (Doyle Rice).
