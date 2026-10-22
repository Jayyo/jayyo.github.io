# jayyo.github.io

Source of https://jayyo.github.io, a single page with clips of the projects on
[github.com/Jayyo](https://github.com/Jayyo) and links to the ones you can run in the
browser.

It is one static `index.html` with no build step. The only outside resource is the
Pretendard web font from jsDelivr. Clips play muted while they are on screen and stay
still for visitors who prefer reduced motion.

`media/` holds the clips and stills. Each clip is cut from that project's own
recording: the Reflow and ChatGPT Navigator clips are short excerpts of their demo
videos (the account email in the Reflow clip is blurred), and the Tongue of War and
Loop Randy clips were recorded from the games in a headless browser.

To preview it locally:

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

Pushing to `main` publishes the page with GitHub Pages
([`.github/workflows/pages.yml`](.github/workflows/pages.yml)).
