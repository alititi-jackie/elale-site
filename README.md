# elale.com — Minimal clothing brand showcase

A lightweight static brand showcase. Chinese is the default language; the header switch toggles English. There is no shopping cart, checkout, account system, or payment.

## Add apparel photos later
1. Put optimized image files in `assets/images/` (prefer WebP, around 1400px on the long edge).
2. Open `assets/js/products.js`.
3. Add an object to `window.ELALE_PRODUCTS` with a bilingual name and image path, for example:

```js
{name:{zh:"新款白色 T 恤",en:"New White T-shirt"},category:"T-SHIRT",tone:"tone-white",image:"/assets/images/white-tee.webp",logo:true}
```

4. Save and deploy. The gallery reads this list automatically; no HTML changes are required.

When real photos are added, make sure the actual garment photo visibly includes the elale logo (ideally a small left-chest embroidery/print). Current artwork is intentionally a temporary CSS placeholder, not a real product photo.

## Main files
- `index.html`: page structure and SEO metadata
- `assets/css/style.css`: layout and visual style
- `assets/js/products.js`: editable apparel gallery list
- `assets/js/main.js`: language toggle, mobile navigation, and gallery rendering
