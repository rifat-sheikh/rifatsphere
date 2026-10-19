# RifatSphere — personal website

A light, natural, bilingual (English + বাংলা) personal website for Rifat Sheik, an aspiring agritech entrepreneur from Bangladesh. Plain HTML, CSS and JavaScript — no framework, no build step, no backend.

## What's in this folder

| File | Purpose |
|---|---|
| `index.html` | The whole website (HTML, CSS and JavaScript in one file) |
| `assets/hero-fallback.svg` | Illustrated rice-field landscape shown behind the hero photo (and if the photo can't load) |
| `assets/rifat-portrait.jpg` | Copy of your portrait (already embedded in `index.html`; use it when changing the photo) |
| `assets/portrait-placeholder.svg` | Spare placeholder image (not used by the page) |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |
| `README.md` | This guide |

## Preview on your computer

Double-click `index.html` to open it in any modern browser. An internet connection is needed to show the hero photo and Google Fonts; without it, the site falls back to the built-in illustration and system fonts.

## Publish on GitHub Pages (existing `rifatsphere` repository)

1. Open your public repository `rifatsphere` on GitHub.
2. Click **Add file → Upload files**.
3. Drag in `index.html`, `.nojekyll`, `README.md` and the whole `assets` folder (unzip this project first). Click **Commit changes**.
4. Go to **Settings → Pages**.
5. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then **Save**.
6. Wait a minute or two, then visit **https://rifat-sheikh.github.io/rifatsphere/**.

> The address assumes your GitHub username is `rifat-sheikh`. If it is different, the address becomes `https://YOUR-USERNAME.github.io/rifatsphere/`. In that case also update the two lines in `index.html` that contain `rifat-sheikh.github.io` (the `canonical` link and `og:url`).
>
> Tip: if the `.nojekyll` file seems hidden on your computer, that is normal — files starting with a dot are hidden by default. Make sure it is included in the upload.

## Change the portrait photo

Your portrait is already embedded directly inside `index.html`, so it shows even if the `assets` folder is not uploaded. A copy is also saved as `assets/rifat-portrait.jpg` (4:5 crop, about 800 × 1000 px).

To use a different photo:

1. Save the new photo (best: 4:5 portrait, about 800 × 1000 px, under ~300 KB) as `assets/rifat-portrait.jpg`.
2. In `index.html`, find the `<img>` inside `<div class="portrait-frame">` and replace its long `src="data:image/jpeg;base64,..."` value with `src="assets/rifat-portrait.jpg"`.
3. Upload both the new photo and `index.html` to GitHub.

## Hero photo

The hero uses a rice-field photo taken in Comilla, Bangladesh by **Injamul Raive**, free to use under the **Unsplash License**, loaded directly from Unsplash. A credit is shown in the footer (not legally required, but kind — please keep it).

Prefer to host the image yourself or use your own photograph?

1. Save the image as `assets/hero.jpg` (about 1920 px wide, ideally under 400 KB).
2. In `index.html`, find the `hero-photo` image and change its `src` to `assets/hero.jpg`.
3. Update or remove the photo credit in the footer (`id="photoCredit"`).

## Edit the content

Everything is in `index.html`. Search for any text to change it. Each English text has a Bangla line (`class="bn"`) directly beneath or beside it.

- Email: search for `mdrifat44057@gmail.com`
- YouTube: search for `youtube.com/@rifatsphere`
- Status labels (Exploring / Learning / Early stage / Planned): inside each card

Research and project cards are honestly labelled **Early stage** or **Planned**. Please update these labels as your work progresses, and only add achievements once they are real.

## Privacy note

Your email address appears publicly on the page. If you prefer, create a dedicated public contact address and swap it in.
