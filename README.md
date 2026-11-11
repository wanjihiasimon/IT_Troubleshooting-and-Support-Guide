# IT Support Field Guide

A searchable, responsive IT troubleshooting reference. The site runs entirely in the browser: it has no login, database, analytics, or backend service. Search, category filters, command copying, and theme preference are client-side; the optional theme choice is stored only in the visitor's browser.

## Run locally with Node.js

Requires Node.js 18 or newer. No dependencies or installation step are needed.

```sh
npm run dev
```

Open <http://localhost:3000>.

## Deploy to Vercel

Import this repository in Vercel and use the **Other** framework preset. Leave the build command and output directory blank; Vercel serves `index.html`, `styles.css`, and `app.js` as static files from the project root. No environment variables are required. The Node server is for local preview only; Vercel's static hosting serves the published site.

## Update the guide

Edit the `guides` array in `app.js`. Each guide includes a category, symptoms, ordered checks, risk level, and optional safety note and vendor reference. Keep steps general, safe, and compatible with your support policy. Verify vendor links periodically.
