# Dog Food Landing Page

This project is a minimal static marketing page built with plain HTML and CSS.

## Tech Stack

- `HTML5` for the page structure and content sections.
- `CSS3` for layout, styling, spacing, colors, and responsiveness.
- Local image assets in [`assets/`](/Users/mac/Desktop/dog-food-landing/assets) for the bowl comparison, dog/product image, feeding GIF, and kibble texture.
- External SVG logo URLs for the payment icons in the hero trust row.

## Project Structure

- [`index.html`](/Users/mac/Desktop/dog-food-landing/index.html)
  Holds the full page structure.
- [`styles.css`](/Users/mac/Desktop/dog-food-landing/styles.css)
  Controls all styling, layout, sizing, and media behavior.
- [`assets/`](/Users/mac/Desktop/dog-food-landing/assets)
  Stores the provided visual assets used on the page.

## How The Site Works

The page is a single static landing page, so there is no framework, build tool, or JavaScript logic involved.

The HTML is divided into clear sections:

- A hero section with:
  the headline, feature blurbs, a split bowl comparison, a call-to-action button, and a trust row.
- A product benefit section:
  text on one side and a real dog/product image on the other.
- A digestion section:
  a feeding animation on one side and supporting text on the other.
- A final section:
  benefit copy paired with a kibble close-up image.

The split bowl effect in the hero is created by placing two bowl images side by side inside a circular container and clipping each image to half of the circle.

## Styling Approach

The CSS uses:

- custom properties in `:root` for shared colors, spacing, and sizing values
- CSS Grid for the main two-column and three-column layouts
- Flexbox for smaller alignment tasks like the CTA stack and trust row
- reusable utility-style classes such as `.container`, `.section`, and `.visual-card`

This keeps the page lightweight and easy to edit without introducing extra tooling.

## Responsiveness

The page is responsive through CSS media queries only.

### Desktop

On large screens:

- the hero uses a three-column layout
- feature cards sit on the left and right of the center bowl
- lower sections use side-by-side text and image blocks

### Tablet

At `max-width: 1080px`:

- the hero collapses into a single-column layout
- the feature cards move into a simpler stacked/grid arrangement
- the lower content sections become one-column blocks

### Mobile

At `max-width: 720px`:

- section padding is reduced
- the hero bowl becomes smaller
- buttons expand to fit the available width
- the trust row stacks vertically
- large visual cards reduce their minimum height for smaller screens

