# Lin Collection

A responsive fashion showcase with a searchable inspiration edit, saved styles and a WhatsApp enquiry bag.

**[Visit the live website](https://lindaodongo.github.io/lincollection.tk/)**

## Overview

Lin Collection presents a fashion edit across dresses, everyday wear, tailoring and accessories. Visitors can explore looks, select preferred sizes and prepare an enquiry without creating an account.

## Features

- Responsive homepage, category sections, style editorial and brand introduction.
- Search and category filters.
- Product detail dialogs with preferred-size selection.
- Saved styles and an enquiry bag stored locally in the browser.
- Quantity adjustments and item removal.
- WhatsApp enquiries containing selected styles, sizes, quantities and an optional delivery town.
- Measurement guidance, delivery and returns FAQs, and privacy information.
- Keyboard-accessible dialogs, enquiry-bag focus handling and reduced-motion support.
- Original shopping-bags homepage photograph, with Black models featured in other fashion imagery.

## Current catalogue status

**The initial collection is an inspiration edit, not live inventory.** Photos and example styles are illustrative; prices, actual designs, sizes, colours and availability must be confirmed directly.

The site does not accept online payments or automatically place orders. Delivery and return arrangements must be agreed before a purchase.

## How the enquiry bag works

1. Open a style and choose a preferred size.
2. Add it to the enquiry bag.
3. Adjust quantities and optionally enter a delivery town.
4. Select **Enquire on WhatsApp**.
5. Review and send the prepared message in WhatsApp.

The enquiry destination is **+254 769 511 266**.

## Technology

HTML5, CSS and vanilla JavaScript, hosted on GitHub Pages. Fonts load from Google Fonts and photographs from Unsplash. No package installation, build process or API keys are required.

## Run locally

```bash
git clone https://github.com/Lindaodongo/lincollection.tk.git
cd lincollection.tk
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). A local server is recommended for predictable browser storage behaviour.

## Customize the storefront

All application code is in `index.html`.

| What to change | Where to edit |
| --- | --- |
| Brand, navigation, page sections and contact details | HTML markup |
| Colours, typography and responsive layout | Embedded `<style>` block |
| Styles, categories, descriptions and photo IDs | JavaScript `products` array |
| Photo URL construction | JavaScript `photo()` helper |
| Product details and enquiry bag | `openProduct()`, `add()` and `renderBag()` |
| WhatsApp message and destination | `sendEnquiry` handler and contact links |
| Size and privacy information | `guide()` and FAQ content |

Use confirmed product details and your own product photography when replacing the inspiration catalogue. Update visible disclosures to match actual inventory and business policies. Add payment processing only through a properly configured provider.

## Storage and privacy

Saved styles use the `lin-saved-v1` local storage key; the enquiry bag uses `lin-bag-v1`. Selections stay in the visitor’s browser and may be unavailable if browser storage is blocked. The privacy dialog includes an option to clear them.

There is no customer database or website payment collection. Visitors choose whether to send their prepared messages through WhatsApp. External image/font providers and GitHub Pages receive ordinary network requests.

## Deployment

GitHub Pages publishes the **`mastor`** branch from **`/ (root)`**. The branch name is spelled `mastor` in this repository.

The `.nojekyll` file enables direct static-file hosting. Commit updates to `mastor` and check the Pages build in the Actions tab.

**Public website:** https://lindaodongo.github.io/lincollection.tk/

The repository name does not itself configure a custom domain. A separate domain requires ownership and DNS configuration.

## Image and font credits

Photographs are hosted by [Unsplash](https://unsplash.com/) and are used as style inspiration, not as endorsements or proof of stock. Fonts are **DM Sans** and **Playfair Display** via [Google Fonts](https://fonts.google.com/). Check applicable asset terms before reusing or replacing them.

## Licence

See [LICENSE](LICENSE) for the repository’s existing MIT licence. Third-party photographs and fonts remain subject to their own licences.

## Contact

**Lin Collection** · [WhatsApp](https://wa.me/254769511266) · 0769 511 266
