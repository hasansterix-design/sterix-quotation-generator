# Sterix Quotation Generator — Installable App

This folder turns the quotation tool into a real app: an icon on your home
screen, opens full-screen with no browser bar, and works completely offline
once installed.

## Why a hosting step is needed (one-time, free)

Phones only allow "install as app" for pages loaded from a real web address
(https://...), not for files opened directly from Files/WhatsApp/email. This
is a phone security rule — not something any app can get around. The good
news: hosting a folder like this is free and takes about 2 minutes, and you
only do it once.

## Step 1 — Put these files online (pick one, both free)

### Option A: GitHub Pages (recommended, most reliable)
1. Go to https://github.com and create a free account if you don't have one.
2. Create a new repository (name it anything, e.g. `sterix-quote`).
3. Upload all the files in this folder (index.html, manifest.json,
   service-worker.js, icon-192.png, icon-512.png, icon-512-maskable.png,
   apple-touch-icon.png) using "Add file → Upload files".
4. Go to the repository's Settings → Pages. Under "Source", choose the
   `main` branch and save.
5. After a minute, GitHub will give you a link like:
   `https://yourusername.github.io/sterix-quote/`
   That's your app's permanent address.

### Option B: Netlify Drop (fastest, no account needed for a quick link)
1. Go to https://app.netlify.com/drop
2. Drag this entire folder onto the page.
3. You'll get a live link immediately (e.g. `https://random-name.netlify.app`).
   For a permanent link that doesn't expire, create a free Netlify account
   and claim the site.

## Step 2 — Install it on your phone

1. Open the link from Step 1 in **Safari** (iPhone) or **Chrome** (Android).
2. **iPhone:** tap the Share icon → "Add to Home Screen" → Add.
   **Android:** tap the ⋮ menu → "Install app" (or you'll see an automatic
   "Install App" button appear inside the page itself).
3. A "Sterix Quote" icon appears on your home screen, exactly like a normal app.

## Step 3 — Use it offline

Open the app from the home screen icon at least once while connected to the
internet (so it can save a copy of itself). After that, it keeps working with
no internet connection at all — product list, calculations, and PDF download
all run entirely on your phone.

## Sharing with your team

Once it's hosted (Step 1), just send everyone the same link. Each person
installs it once on their own phone using Step 2, and from then on it's their
own offline app icon.

## Updating prices later

If the price list changes, edit `index.html` (the PRODUCTS list near the top
of the `<script>` section) and re-upload just that file to the same hosting.
Everyone's installed app will pick up the update automatically next time
they open it with internet access.
