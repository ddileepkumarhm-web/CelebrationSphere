# CelebrationSphere — Event Planning & Celebration Booking Platform

A polished React single-page application for discovering, customising and requesting celebration packages. This project is an original, enhanced implementation inspired by the supplied CelebrationCraft reference assignment.

## Highlights
- Responsive landing page and occasion-based discovery
- Search, category filtering, budget filtering and price sorting
- Package detail pages with included features and save/favourite action
- Booking request form with validation and confirmation
- Booking history with reference IDs and status
- Create/publish custom event packages with live preview
- Persistent events, bookings and favourites using browser `localStorage`
- React Router navigation, accessible labels, skip link, empty states and 404 page
- Unit/integration test setup with Vitest and React Testing Library

## Requirements
- Node.js 18 or newer
- npm

## Run locally
1. Extract the ZIP file.
2. Open a terminal in the `CelebrationSphere` folder (the folder containing `package.json`).
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```
5. Open the URL printed by Vite, usually `http://localhost:5173`.

## Verify
```bash
npm test
npm run build
```

## Main routes
| Route | Purpose |
|---|---|
| `/` | Landing page and featured experiences |
| `/events` | Searchable and filterable package catalogue |
| `/events/:id` | Package detail and booking entry |
| `/book` | Booking request form |
| `/bookings` | Booking history |
| `/create` | Create and publish a custom package |

## Project structure
```text
CelebrationSphere/
├── public/
├── src/
│   ├── components/       Reusable navigation, cards and headings
│   ├── context/          Shared application state and localStorage
│   ├── data/             Occasion categories and starter packages
│   ├── pages/            Home, catalogue, details, booking, history, create, 404
│   ├── test/             Test setup
│   ├── utils/            Formatting and validation helpers
│   ├── App.jsx
│   ├── App.test.jsx
│   ├── main.jsx
│   └── styles.css
├── index.html
├── package.json
└── vite.config.js
```

## Data and limitations
This is a front-end academic demonstration. Data is saved in the browser's local storage on the device/browser used. It does not connect to a live payment gateway, email service, server database or real event inventory. Package images are loaded from Unsplash and therefore require an internet connection. Booking requests are demonstration records, not actual reservations.

## Suggested demonstration flow
1. Browse featured experiences on the home page.
2. Open Explore, search for an occasion and apply a budget filter.
3. Open a package detail page and save it to favourites.
4. Submit a booking request using a future date.
5. Visit My bookings to show the saved booking.
6. Open Plan an event, create a custom package and publish it.
7. Return to Explore and show the newly published package.
