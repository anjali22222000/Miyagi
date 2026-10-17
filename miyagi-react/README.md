# Miyagi — Speaker & Events (React + Vite, frontend demo)

## Run
```
npm install
npm run dev        # http://localhost:5173
npm run build      # production build in dist/
npm run preview
```

## Admin
Open `/#/admin` — demo login `admin@miyagi.demo` / `miyagi123`.
Frontend-only demo session, NOT secure authentication.

## Structure
- `src/data/seed.js` sample events and posts · `store.js` localStorage + `useData` hook · `programs.js` program data
- `src/components/` Scene (illustrated artwork), Bokeh (canvas particles), Footer, shared UI and forms
- `src/pages/` Home, PublicPages (About, Team, Programs, Events, Blog, Contact...), Admin
- `src/layouts/PublicLayout.jsx` public header/footer shell
- `src/App.jsx` hash router · `src/styles/main.css` all styles

## Notes
- Routing uses a small hash router (`#/events/e1`), so it works on any static host.
- Data lives in localStorage; clear site data to reset the sample content.
- Payments are simulated; no real money is charged. All people, testimonials and events are fictional.
- Images are illustrated SVG scenes. To use photos, paste URLs into the poster/image fields in admin or edit `src/data/seed.js`.
