# Uke School

A pocket practice ukulele in a single web page: a live tuner dial, colour-coded chord cards that check your chord through the microphone, a strumming metronome, play-along songs and a one-minute chord-change drill.

No build step and no dependencies. Everything lives in `index.html`.

## Run it on your computer

### 1. Get the files

With [GitHub Desktop](https://desktop.github.com): **File → Clone repository → JensonNg/ukulele**.

Or in Terminal:

```bash
git clone https://github.com/JensonNg/ukulele.git
cd ukulele
```

### 2. Open it

**Quick look:** double-click `index.html`. Chords, strumming, songs and practice all work this way.

**With the microphone (tuner and "Check my chord"):** browsers only allow the mic on a proper web address, so start a small local server from inside the `ukulele` folder:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000> in Chrome, Safari or Firefox and allow microphone access. Press `Ctrl + C` in Terminal to stop the server.

### 3. Make changes

Edit `index.html`, save, and refresh the browser. When you're happy:

```bash
git add .
git commit -m "Describe what you changed"
git push
```

Pushing only updates the private repo on GitHub. Nothing goes public until you do the next step.

## Publish it as a portfolio piece (later)

GitHub Pages can host this page for free:

1. On GitHub, open the repo → **Settings → General → Danger Zone → Change visibility → Public**. (Free accounts can only publish public repos.)
2. **Settings → Pages → Build and deployment → Deploy from a branch**, pick the default branch and `/ (root)`, then **Save**.
3. After a minute it is live at `https://jensonng.github.io/ukulele/`. You can link it from your portfolio site.

## Privacy

Recordings and practice scores stay in the visitor's own browser. Nothing is uploaded anywhere.
