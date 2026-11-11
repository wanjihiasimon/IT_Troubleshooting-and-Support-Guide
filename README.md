# IT Support Field Guide

A searchable, responsive IT troubleshooting reference. The site runs entirely in the browser: it has no login, database, analytics, or backend service. Search, category filters, command copying, and theme preference are client-side; the optional theme choice is stored only in the visitor's browser.

## Run locally with Node.js

Requires Node.js 18 or newer. No dependencies or installation step are needed.

```sh
npm run dev
```

Open <http://localhost:3000>.

## Deploy to Vercel

The repository config pins the **Other** framework preset, disables the build command, and publishes only the `public/` directory. Import the repository and redeploy; no environment variables are required. `server.js` is for local preview only and is outside the published output. The site files to edit are `public/index.html`, `public/styles.css`, and `public/app.js`.

## Update the guide

Edit the `guides` array in `app.js`. Each guide includes a category, symptoms, ordered checks, risk level, and optional safety note and vendor reference. Keep steps general, safe, and compatible with your support policy. Verify vendor links periodically.
