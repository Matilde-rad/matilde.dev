# matilde.dev

My personal portfolio site: experience, education and projects.

Live at [matilde.dev](https://matilde.dev).

## What it is

A single static page, written in plain HTML and CSS with a little JavaScript for the scroll reveals and the soft background colours. There is no build step and no dependencies.

## Files

- `wrangler.jsonc`: Cloudflare config (publishes the `public` folder)
- `public/index.html`: the whole page (markup, styles and script)
- `public/intapp.png`, `public/ltplabs.png`, `public/car.png`: logos and photo used in the Experience section

## Run it locally

Open `public/index.html` in a browser. Or serve the folder:

```
python -m http.server 8000 --directory public
```

then visit http://localhost:8000.

## Deploy

Hosted on Cloudflare, connected to this repo. Pushing to `main` redeploys the site.

## Notes

The Echoflow block links to `echoflow.matilde.dev` but is marked `soon` until that site is live. To switch it on, remove `soon` from the class on `<a class="project soon ...">` in `index.html`.
