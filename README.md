# GuitarTuner

A lightweight, browser-based guitar tuner by **dw-creative**.

Live version: https://dw-creative.github.io/guitartuner/

## Features

- Chromatic tuning mode
- Beginner mode with manual string selection
- Clear beginner guidance: **TIGHTEN**, **LOOSEN**, or **IN TUNE**
- Standard guitar tuning from low E to high E
- Sensitive microphone input for acoustic, classical, and unamplified electric guitars
- Stabilized pitch detection to reduce needle movement during the initial attack of a plucked string
- Adjustable A4 reference pitch, defaulting to 440 Hz
- Automatic microphone startup where the browser allows it
- Non-blocking fallback if the browser requires a tap before starting audio
- Optimized for iPhone and standalone Home Screen use
- Works on modern desktop and mobile browsers
- No server-side processing: microphone audio is analyzed locally in the browser

## Languages

The interface follows the browser / system language by default:

- **German** for devices whose preferred language starts with `de`
- **English** for all other languages

You can also override the language manually in **Settings → Language** and choose:

- **Automatic**
- **Deutsch**
- **English**

The selected preference is stored locally in the browser.

German note naming uses **H**.  
English note naming uses **B**.

## Beginner mode

The strings are numbered from thickest to thinnest:

1. Low E
2. A
3. D
4. G
5. B
6. High E

Select the string you want to tune and pluck it. The tuner compares the detected pitch directly with the selected target string, even when the current pitch is several semitones away.

The app then gives a simple instruction:

- **TIGHTEN ↑** — the string is too low
- **LOOSEN ↓** — the string is too high
- **IN TUNE ✓** — the string is correctly tuned

## Browser requirements

Microphone access requires a secure context:

- HTTPS, such as GitHub Pages
- or `localhost` for local development

Opening `index.html` directly through a `file://` URL may prevent microphone access in some browsers.

## iPhone / Home Screen

Open the live site in Safari, then choose:

**Share → Add to Home Screen**

The layout is designed to fit an iPhone display in standalone mode without requiring vertical scrolling.

## Deployment with GitHub Pages

This project is intentionally simple and does not need a build process.

Repository contents:

```text
guitartuner/
├── index.html
└── README.md
```

To publish it with GitHub Pages:

1. Open **Settings → Pages** in the repository.
2. Select **Deploy from a branch**.
3. Choose the `main` branch.
4. Choose `/ (root)`.
5. Save.

The site will then be available at:

https://dw-creative.github.io/guitartuner/

## Privacy

Audio from the microphone is processed locally in the browser using the Web Audio API. The app does not upload or store microphone audio.

## License

No license has been added yet. Add a license file if you want others to reuse or redistribute the source code under defined terms.
