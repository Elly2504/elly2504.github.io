# elly2504.github.io

Static site published with GitHub Pages. It hosts the App Store-required
support, privacy and terms pages for the iOS apps listed on the home page.

Plain HTML + one stylesheet. No build step, no dependencies, no JavaScript.
`.nojekyll` is present so files are served exactly as committed.

```
/                       app index
/assets/                style.css, icon, mascots
/dentalingo/            Dentalingo — marketing / overview page
/dentalingo/support/    App Store "Support URL"
/dentalingo/privacy/    App Store "Privacy Policy URL"
/dentalingo/terms/      Terms of Use (Apple standard EULA + app-specific terms)
/dentalingo/credits/    Open-source, image and audio attributions
```

## Editing

Edit the HTML and push to `main`; Pages redeploys in about a minute.
Every page repeats the same header, footer and DANB trademark notice — if you
change one, change all five.

## Local preview

```sh
python3 -m http.server 8000
# http://localhost:8000/dentalingo/
```
