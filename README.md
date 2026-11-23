# SOMNA — The Sleep Studio

A **free, private, iPhone-friendly sleep studio** with 88 techniques, 12 original device-narrated hypnosis-style journeys with adjustable repeat length, 12 customizable procedural soundscapes, a sleep-stack builder, CBT-I-informed guides, a breathing coach, cognitive shuffle, thought parking, and optional sleep journaling.

## Run on iPhone without a computer

**Best route: GitHub Pages from Safari on iPhone.** A computer, Apple developer account or App Store submission is not required.

1. Unzip the package in the iPhone **Files** app.
2. Open **github.com** in Safari and sign in. Create a **public repository** named `somna-sleep-studio` (or another name).
3. In that repository choose **Add file → Upload files**, then upload `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png` and `icon-512.png` from Files. All should be in the repository **root**, not inside another folder. If Safari shows the mobile GitHub site without Upload files, request **Desktop Website** from Safari's page controls.
4. In repository **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, branch `main` and folder `/ (root)`; save. Wait for GitHub to show your Pages site URL (usually `https://USERNAME.github.io/somna-sleep-studio/`).
5. Open the site in **Safari**, tap **Share → Add to Home Screen → Add**. Launch **SOMNA** from its new icon. The service worker caches its files after the first successful load, for offline use.

The downloaded `index.html` is also a **single-file version** that contains the full application code; whether your iPhone opens interactive local HTML directly depends on the Files preview/browser behavior. Hosting on GitHub Pages is more reliable for iPhone audio and home-screen mode.

## What works offline?

Method library, search and filters, local notes, journal, breathing guides, colors, original scripts and soundscapes work without servers after caching. **Spoken narration** uses Safari/iOS `speechSynthesis` voices available on your phone; voice availability varies and a voice might first need downloading in iOS. The **soundscapes** are synthesized using Web Audio, not music files. Audio may pause when the iPhone locks or when the app is backgrounded, depending on iOS and the browser. For best results keep the screen active at its lowest comfortable brightness with Auto-Lock set appropriately, or use iOS's own background audio player for locked-screen audio.

The app cannot change actual iPhone system brightness, Do Not Disturb, or Auto-Lock. Night focus only changes the app display. No cloud account, subscriptions, tracking, user-data uploads, or paid APIs are used.

## Audio caution and limitations

Voice sessions are **original relaxation/hypnosis-style scripts** (you can repeat each passage 1–4 times to extend the audio) narrated using your device's built-in voices, not studio-recorded MP3s. Effects vary, and no method is guaranteed to make you fall asleep rapidly. Sound masking, binaural or hypnosis claims should not be confused with validated treatment. Keep volume low and never use while driving. Avoid breath holds if uncomfortable or dizzy. If insomnia is persistent, CBT-I is an evidence-based treatment; consult a clinician if needed.

## Tech

- Vanilla HTML/CSS/JS, no dependencies or external CDNs.
- Browser localStorage for settings, notes and diary; manual JSON export/import supported.
- Web Speech API for narrated scripts, Web Audio API for procedural sound layers.
- PWA manifest, icons and service worker for HTTPS installation/offline cache.
- WCAG-oriented touch targets, responsive UI and reduced-motion options.

## Research references

- [AASM behavioral and psychological treatments for insomnia](https://pmc.ncbi.nlm.nih.gov/articles/PMC7853203/)
- [NHS insomnia](https://www.nhs.uk/conditions/insomnia/)
- [NCCIH sleep disorders and complementary approaches](https://www.nccih.nih.gov/health/sleep-disorders-and-complementary-health-approaches)
- [Systematic review of hypnotherapy for sleep](https://pubmed.ncbi.nlm.nih.gov/37399315/)
- [Systematic review of noise as a sleep aid](https://pubmed.ncbi.nlm.nih.gov/33007706/)

© 2026 — Original code, narration and design made for this request.
