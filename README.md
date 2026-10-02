# VR Menu Showcase

A historical A-Frame scene that arranges menu images in a virtual environment.
[`index.html`](index.html) contains the scene and asset references; `img/` holds
the menu textures. This is a visual experiment, not an ordering/payment service.

## Preview

No compilation is required. With Python 3, run from the repository root:

```sh
python -m http.server 7000 --bind 127.0.0.1
```

Open `http://127.0.0.1:7000` and stop with Ctrl+C. Alternatively, the committed
Node workflow is `npm ci` followed by `npm start`, which starts Live Server on
port 7000. The historical npm install was not revalidated in this review.

The page loads A-Frame 0.9.2 and ground/sky textures from external hosts, so the
static preview needs those assets to remain reachable. Desktop scene viewing
does not verify headset, WebXR, keyboard or mobile compatibility. No automated
test suite, CI workflow or runtime environment variables are configured.

The `deploy` script publishes through `ghpages`; it is not a local preview or
verification command and was not run for this review.

## Attribution and contributions

Built with [A-Frame](https://aframe.io). Preserve the existing [MIT license](LICENSE)
and any upstream asset attribution. The menu image ownership/redistribution
rights have not been independently audited; the source license does not establish
rights to every depicted brand or supplied image. For changes, include the actual
browser/device tested and check texture loading and scene navigation.
