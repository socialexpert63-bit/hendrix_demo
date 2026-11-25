# Hendrix R&D360 – Demo Prototype

A concept dashboard for digital R&D (research, testing and certification) built with **demonstration data**. It is a proposed concept, not a Hendrix product.

When the dashboard opens, a branded splash screen ("Prepared for Eladio Piñero González") invites the client to watch a 75-second overview. One click starts the video with an AI voiceover narrating each screen.

## Project structure

```
hendrix-rd360-demo/
├── index.html              # The dashboard (self-contained, includes the splash and the embedded video)
├── video/
│   └── concept-video.html  # The standalone 75-second concept video
├── assets/
│   └── voiceover.mp3       # AI voiceover track (already embedded in both HTML files; kept for reference)
├── .nojekyll               # Lets GitHub Pages serve the files as they are
├── .gitignore
└── README.md
```

## Run locally

No build step or dependencies. Open `index.html` in a desktop browser (Chrome or Edge recommended).

## Deploy with GitHub Pages

1. Create a new repository on GitHub and upload the contents of this folder (or push it with git).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. After a minute, the site is live at `https://<your-username>.github.io/<repository-name>/`.

The standalone video will be at `.../video/concept-video.html`.

## Notes

- Browsers only allow sound after a click. That is why the splash screen asks the client to click once to watch the overview; the AI voice then plays automatically.
- Everything is embedded in the HTML files, so the project also works offline and can be sent as a single file.
- Fonts (Cormorant Garamond, Raleway, Manrope) load from Google Fonts when online and fall back to system fonts otherwise.
- All data shown is fictional demonstration data.

## Changing the client name

Open `index.html`, search for `Eladio`, and replace the name in the splash screen and in the video window title.

## Video controls (standalone video)

Space = play/pause · R = restart · M = mute · H = hide controls · Left/Right = seek 5 seconds.
