# ANIIS SHOES

A premium, fully responsive sneaker storefront concept with a live cloud order desk.

- Six houses: Nike, adidas, Jordan, PUMA, New Balance, ASICS
- 18 curated colorways with smooth color transitions
- Interactive 3D shoe tilt, quick view, search, filters, wishlist, cart and checkout
- Firebase Auth + Firestore order storage with offline retry
- Protected studio order desk: live orders, revenue, fulfilment status and CSV export
- Sync centre with customer cloud receipts, Google sign-in and order tracking
- All fonts, images and styles embedded in a single self-contained page
- Optimized for phones, tablets, desktops and landscape screens

## Live sites

- Firebase Hosting: https://aniis-shoes.web.app/
- GitHub Pages: https://pedrodxs.github.io/aniis-shoes/

## Cloud orders

Orders are stored in Google Cloud Firestore under the `orders` collection and protected by Firebase security rules. The storefront uses an anonymous Firebase session for guest checkout. Only order details are saved; card details never leave the browser.

The studio order desk is available from the footer or the sync centre. Access is restricted to the owner account configured in `firestore.rules`.

## Run locally

Open `index.html` directly in a browser for the offline storefront preview. Cloud sync requires the hosted site.

---

Concept storefront for demonstration purposes. Payment is simulated. Product photography belongs to the respective brands.

