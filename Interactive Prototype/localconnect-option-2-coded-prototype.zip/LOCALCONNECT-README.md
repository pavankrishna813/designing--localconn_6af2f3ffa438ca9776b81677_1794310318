# LocalConnect — Option 2 coded prototype

Prepared 10 November 2026. Selected by the user: blue map-first direction.

## Package contents

The prototype ZIP includes runnable React/TypeScript source, the lockfile, generated image assets, the protected mobile runtime, the production build, and design QA notes. The screen ZIP contains five critical screen exports and additional tested states.

## Run

In the extracted source folder run `npm ci`, then `npm run dev -- --host localhost --port 4173`. Open `http://localhost:4173/`. Dependencies require Node/npm. The prebuilt `dist/client` can also be served by an ordinary static HTTP server; opening index.html directly from disk is unsupported because assets use site-relative paths.

## What works

Discover sample events from the map or list; search and recover from no results; select date and location; view practical event information; save and retrieve events; enter sample registration details; recover from validation errors; confirm a reservation; retrieve and cancel it in My events. iPhone and Pixel previews are provided by the template.

## Evidence and limitations

Production build and runtime integrity checks passed. Browser checks covered the primary flow and recovery states. QA is technical/design verification by the assistant, **not participant usability research**.

All events, organisers, venues and access details are fictional. Use sample details. Reservation/saved state exists only in memory and clears on refresh; no email or real booking is created. The map is an illustration rather than a navigation service.

**This coded prototype is not a Figma prototype.** The assignment explicitly asks for Figma; a viewable Figma file and real research/usability evidence are still required for full completion. Uploading this package does not establish that those requirements are satisfied.
