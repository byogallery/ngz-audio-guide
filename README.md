# National Gallery of Zimbabwe — Bulawayo Audio Guide

Mobile-first, static audio guide website for GitHub Pages. No installation, paid hosting, analytics or third-party scripts required.

## Included

- `index.html` — website
- `style.css` — layout, colors and responsive mobile styling
- `app.js` — chapter navigation, playback, scrubbing and transcript interaction
- `chapters.js` — 11 chapter titles, text, and audio file paths
- `images/gallery-exterior.jpg` — user-supplied exterior photo
- `audio/02.m4a` etc. — nine real audio files (chapters 2–4 and 6–11)

Chapter 1 and chapter 5 currently show “Audio coming soon”. Chapter 12 is intentionally omitted.

## Publish on GitHub Pages (no coding required)

1. Sign in to https://github.com/ and choose **New repository**.
2. Name the repository `ngz-audio-guide`, choose **Public**, then click **Create repository**.
3. On the repository's **Code** page choose **Add file → Upload files**.
4. Upload **the contents of this folder** to the repository root. `index.html`, `app.js`, `style.css`, and `chapters.js` must be at the top level, with `audio/` and `images/` folders intact. Upload individual files and folders, not the ZIP file itself. Desktop web GitHub supports dragging the complete folder content into the upload box; if using a phone, a desktop/laptop may be easier for the bulk upload.
5. Click **Commit changes**.
6. Go to **Settings → Pages**. In **Build and deployment**, choose **Deploy from a branch**; branch **main**, folder **/(root)**; click **Save**.
7. After the deployment completes, open the **Visit site** link on the Pages settings screen. Typical address: `https://YOUR-USERNAME.github.io/ngz-audio-guide/`.
8. Open it on both iPhone (Safari) and Android (Chrome); play chapter 2, move the seek bar, open a transcript and switch to chapter 3.

## Replacing audio

Export recordings as `.m4a` AAC, preferably mono 96–128 kbps for lighter mobile data usage. Rename files `01.m4a` and `05.m4a`, put them in `audio/`, and edit the matching entries in `chapters.js` from `audio:null,duration:null` to `audio:'audio/01.m4a',duration:'M:SS'` or `audio:'audio/05.m4a',duration:'M:SS'` respectively. Keep names lower-case and use exact matching paths.

## Changing photos

Replace `images/gallery-exterior.jpg` with a landscape photo of the same filename. The current chapter thumbnails other than chapter 2 are illustrated placeholders. To add individual real chapter photos, ask for an update to the website code; please ensure you have permission to publish them.

## Important

- Audio starts only after a visitor taps Play (iOS/Android browser requirement).
- Audio streams over the internet; headphones recommended.
- Browsers may pause sound when the screen locks, an incoming call occurs, or another app takes focus. Background playback behavior varies by browser.
- This is a public website; only upload photos/audio that the Gallery is allowed to publish.
- The gallery logo is a **temporary typographic placeholder**, not an official logo. Replace it with the approved logo before public launch.
- Transcripts are based on the supplied draft script and should be proofread against the finalized recordings before public launch.
- No automatic translation is built in. The current guide is English only.
- Site design can be tested by opening `index.html` locally, but published HTTPS GitHub Pages is the definitive mobile playback test.
