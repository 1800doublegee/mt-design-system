# MT Font Assets

Add licensed font files to the subfolders below.

## Items MT Light — `Items-MT-Light/`

**Foundry:** Colophon Foundry (custom commission for Made Thought)
**Weight:** Light (300)
**Classification:** Contemporary serif with humanist details

Required files (add whichever formats you have):
- `ItemsMT-Light.otf`
- `ItemsMT-Light.woff2`
- `ItemsMT-Light.ttf`

**Note:** Items MT is a proprietary typeface commissioned by Made Thought from Colophon Foundry.
It is not publicly available. Files must be sourced from the MT type library.

---

## Futura PT Book — `Futura-PT-Book/`

**Foundry:** ParaType (Futura PT is the digitisation of Paul Renner's Futura)
**Weight:** Book (400), Demi (600)
**Classification:** Geometric sans-serif

Required files:
- `FuturaPT-Book.otf`
- `FuturaPT-Book.woff2`
- `FuturaPT-Demi.otf`
- `FuturaPT-Demi.woff2`

Futura PT Book is available via:
- Adobe Fonts (if MT has an Adobe CC subscription)
- Linotype (purchase)
- ParaType direct

---

## Fallback stack (if fonts are unavailable)

```css
/* Display — if Items MT is missing */
font-family: 'Playfair Display', 'Cormorant Garamond', Georgia, serif;

/* UI — if Futura PT is missing */
font-family: 'Helvetica Neue', 'Arial', sans-serif;
```

Note: Fallback fonts will not produce authentic MT output.
Font files must be present for production-quality work.
