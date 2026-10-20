# ANIIS SHOES

A premium, fully responsive sneaker storefront with a separate private studio for order management.

- Six houses: Nike, adidas, Jordan, PUMA, New Balance, ASICS
- 18 curated colorways with smooth color transitions
- Interactive 3D shoe tilt, quick view, search, filters, wishlist, cart and checkout
- Firebase Auth + Firestore order storage with offline retry
- Separate studio portal: live orders, revenue, fulfilment status and CSV export
- Customer sync centre with cloud receipts, Google sign-in and order tracking
- All fonts, images and styles embedded in self-contained pages
- Optimized for phones, tablets, desktops and landscape screens

## Live sites

- Customer storefront: https://aniis-shoes.web.app/
- Studio order desk: https://aniis-shoes.web.app/studio
- GitHub storefront: https://pedrodxs.github.io/aniis-shoes/
- GitHub studio: https://pedrodxs.github.io/aniis-shoes/studio.html

The studio is a separate, noindex portal and is not linked from the customer storefront. It is protected by Firebase Auth and Firestore security rules.

## Cloud orders

Orders are stored in Google Cloud Firestore under the `orders` collection and protected by Firebase security rules. The storefront uses an anonymous Firebase session for guest checkout. Only order details are saved; card details never leave the browser.

Customers can sign in with Google in the sync centre to keep their order history. Studio access is restricted to the owner account configured in `firestore.rules`.

## Run locally

Open `index.html` directly in a browser for the offline storefront preview. Cloud sync requires the hosted site.

---

Concept storefront for demonstration purposes. Payment is simulated. Product photography belongs to the respective brands.
