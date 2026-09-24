# The Kingslayer Resort · Website

A static one-page site for The Kingslayer Resort, Negombo. It's ready to host on **Vercel**. There's no build step and nothing to install.

```
kingslayer-resort/
├── index.html            ← the website
├── img/                  ← 10 property photos (optimised JPGs)
├── favicon.svg           ← browser tab icon (gold crown)
├── apple-touch-icon.png  ← home-screen icon for iPhone/Android
├── 404.html              ← branded "page not found"
├── robots.txt            ← lets Google index the site
└── vercel.json           ← clean URLs, image caching, security headers
```

---

## Deploy to Vercel

> Vercel doesn't accept a zip upload directly. Unzip this folder first, then use **one** of the options below.

### Option A: GitHub + Vercel (easiest, no coding)
1. Unzip this file.
2. Go to **github.com**, then **New repository** (e.g. `kingslayer-resort`), then **Create**.
3. Click **"uploading an existing file"** and drag in **everything inside** the `kingslayer-resort` folder (`index.html`, `img/`, `vercel.json` and the rest). Commit.
4. Go to **vercel.com/new**, then **Import** that repository.
   - Framework Preset: **Other**
   - Build Command: *(leave empty)*
   - Output Directory: *(leave empty / root)*
5. Click **Deploy**. You'll get a live link like `kingslayer-resort.vercel.app`.

From then on, any change you push to GitHub goes live automatically.

### Option B: Vercel CLI (terminal)
```bash
npm i -g vercel
cd kingslayer-resort
vercel          # first time: log in and accept the defaults
vercel --prod   # publish to production
```

---

## After it's live
1. **Custom domain** (e.g. `kingslayerresort.lk`): in Vercel go to **Project**, then **Settings**, then **Domains**, then **Add**, and follow the DNS instructions.
2. **Social share image**: open `index.html` and change
   `<meta property="og:image" content="img/pool-house.jpg">`
   to the full URL, e.g. `https://YOUR-DOMAIN/img/pool-house.jpg`, so WhatsApp and Facebook link previews show the pool photo.
3. **Google Business Profile**: add the new website URL so guests find it from Google Maps.

## Quick edits (in `index.html`)
| What | Search for |
|---|---|
| WhatsApp / phone number | `94719393266` |
| Room prices | `US$30`, `US$34` |
| Room text | `Deluxe Double or Twin` |
| Reviews | `class="rev"` |
| Languages spoken | `English · Tamil` |

Contact: +94 71 939 3266 · 21/3 Palagathura Lane, Kochchikade, Negombo 11540
