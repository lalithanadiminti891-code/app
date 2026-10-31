# Nadiminti's Classic Food

## Start on Windows
1. Install the current LTS version of Node.js from https://nodejs.org.
2. Extract this ZIP, then open the `app` folder in VS Code.
3. Copy `.env.example` to a new file named `.env`, then set a private `ADMIN_KEY`.
4. Open the VS Code terminal and run `npm start`, then open http://localhost:3000 in your browser.

This package has no external libraries, so no `npm install` step is required.

Customer ordering is at `/`; the order dashboard is at `/admin.html` and requires the `ADMIN_KEY`.

## Included delivery rules
- Delivery uses the customer's browser GPS and approximate Shyamalamba Thalli Temple coordinates.
- 0–2 km: ₹20; over 2–4 km: ₹30; over 4–7 km: ₹40; more than 7 km: unavailable.
- Takeaway has no delivery charge.

For public use, host the site over HTTPS because browsers restrict GPS on ordinary HTTP websites. The distance is straight-line, not driving distance. Confirm the restaurant entrance GPS coordinates before launch.
