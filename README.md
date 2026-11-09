# Ascentium SME platform (concept prototype)

Static site: one `index.html` plus 21 startup-toolkit PDFs in `toolkits/`. No build step.

## Deploy to Vercel

**Option A: Vercel CLI**
1. Install Node.js, then run `npm i -g vercel`
2. In this folder, run `vercel` (first time: log in and accept the defaults)
3. Run `vercel --prod` to publish to production

**Option B: GitHub**
1. Push this folder to a new GitHub repository
2. On vercel.com, choose Add New > Project and import the repository
3. Framework preset: Other. Build command: none. Output directory: `.` (root)
4. Deploy

## Notes
- Pages are hash routes (for example `/#pricing`), so no rewrites are needed.
- The product tour remembers progress in the browser's localStorage.
- Fonts load from Google Fonts; everything else is self-contained.
- This is a concept prototype: forms send nothing and pricing is indicative.
