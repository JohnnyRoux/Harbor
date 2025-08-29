
# Harbor — Directory MVP (Next.js + Tailwind on Vercel)

A small 3-page app you can deploy free to Vercel. Import your companies via CSV (stored in the browser) and browse results with filters.

## Features
- Home, Browse (Results), Company Profile, Pricing, Import CSV
- Client-side search + filters
- CSV importer (uses PapaParse) and saves to `localStorage`
- Tailwind styling, clean and responsive

## Quick Start (Local)
1. Install Node 18+
2. `npm install`
3. `npm run dev`
4. Open http://localhost:3000

## Deploy to Vercel (Free)
1. Create a GitHub repo and push this folder.
2. Go to https://vercel.com → “Add New Project” → Import your repo.
3. Framework Preset: **Next.js** (detected automatically).
4. Environment/Build settings: defaults are fine. Click **Deploy**.
5. Open your live URL → go to `/import` to upload your CSV and save to the browser.

## Importing data
- Use the **Import CSV** page or download the template from `/import`.
- After import, the **Browse** page reads from your browser data. (If nothing imported, it falls back to sample data.)

## Next steps (optional)
- Swap `localStorage` for a real database (Supabase) and add Auth.
- Add an “Edit Listing” screen for owners.
- Add payments (Stripe) for Pro/Partner tiers.

---

**Note**: This MVP stores imported data only in your browser for demo simplicity. For multi-user, you'll connect to a database.
