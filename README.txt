MCQ Master - mobile web app (PWA)

FILES
  index.html, script.js, style.css     the app
  sw.js, manifest.webmanifest,   make it installable + offline
  q-manifest.js, q-*.js                your questions
  check.html                           data checker (open it to validate the q-*.js files)

HOW TO USE
  1. Upload the whole folder to any HTTPS host (GitHub Pages, Netlify, Cloudflare Pages, Vercel).
     Installing and offline mode do not work from file://. For a local test run:
        python3 -m http.server 8000      then open http://localhost:8000
  2. Open the site on your phone:
        Android/Chrome: tap the "Install" card (or browser menu > Install app)
        iPhone/Safari : Share > Add to Home Screen

UPDATING QUESTIONS
  Edit/add q-*.js, update q-manifest.js, and change the "v" number in q-manifest.js.
  Phones then download the new data automatically and show a "new version" bar.

WHAT'S NEW
  - Exam setup page redesigned (summary tiles, steppers, cut-mark selector).
  - More > MCQ AI: chat that reads the whole question bank (works offline).
    Optional: tap the gear and add an OpenAI-compatible API key to answer anything.
  - More > Question Slider: timed slideshow (30/60/90/120 s), answer + explanation, swipe or arrow keys.
  - General Knowledge (English) category removed; Math added (Arithmetic, Algebra, Geometry, Mensuration).

NOTE
  q-manifest.js lists files (q-s5.js ... q-s15.js, q-sgd.js) that were not in the upload.
  Keep them next to the other q-*.js files or the app skips those lessons.
