<div align="center">
  <img src="docs/preview.jpg" alt="Blueprint — a portfolio drawn as a technical drawing" width="100%">
</div>

<h1 align="center">Blueprint</h1>

<p align="center"><em>A portfolio presented as a technical drawing.</em></p>

<p align="center">
  <a href="https://noxwer-beep.github.io/blueprint/">Live</a> ·
  <a href="https://noxwer-beep.github.io/showcase/">All eight concepts</a> ·
  <a href="https://noxwer-beep.github.io/portfolio/">Portfolio</a>
</p>

---

I wanted to see whether a page can explain itself the way a drawing does: dimensions,
leader lines, a title block, the construction grid left visible. So the content is
annotated instead of decorated.

## What is in here

```
index.html   structure, and the sheet annotations
style.css    the drawing: rules, hatching, dimension marks
main.js      scroll reveals and the pointer-driven sheet details
css/         self-hosted fonts (Space Grotesk, IBM Plex Mono, Fraunces)
```

Three files, no framework, no build step, no bundler. Open `index.html` and it works.

## Run it

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## What it demonstrates

- **Annotation as layout.** Labels sit on leader lines and the grid stays visible, so
  you can see how the page was put together.
- **`IntersectionObserver` reveals** that fire once and never re-run. It settles
  instead of animating forever.
- **Pointer position as a CSS variable**, so the sheet reacts to the cursor without an
  animation frame running when nobody is looking.

## Related

- [showcase](https://github.com/Noxwer-beep/showcase) — the gallery these came from,
  with the design notes for each direction
- [portfolio](https://github.com/Noxwer-beep/portfolio) — the real site

MIT.
