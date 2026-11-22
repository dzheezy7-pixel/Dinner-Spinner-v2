DINNER SPINNER - installable app
================================

Files in this folder:
  index.html            the app
  manifest.webmanifest  tells phones it is an installable app
  sw.js                 lets it work offline
  icon-*.png, apple-touch-icon.png   app icons

STEP 1 - Put the folder online (free, ~2 minutes)
Apps must be served over https, so upload the whole folder to a free host:

  Easiest: Netlify Drop
    1. Unzip this file.
    2. Go to https://app.netlify.com/drop
    3. Drag the unzipped folder onto the page.
    4. You get a link like https://something.netlify.app

  Also works: GitHub Pages or Cloudflare Pages (upload these files as-is).

STEP 2 - Install it on your phone
  iPhone (use Safari):  Share button -> Add to Home Screen
  Android (use Chrome): menu (three dots) -> Install app / Add to Home screen
  Desktop Chrome/Edge:  install icon at the right end of the address bar

After installing, it opens full screen with its own icon and works offline.
Your added and removed options are saved on that device.

Updating later: change the files, re-upload, and bump the version number
in sw.js (CACHE = 'dinner-spinner-v2') so installed copies refresh.
