# ASL Bethel Jobs

A Deaf-friendly job board. Made by Tyree and Kianu.

Stack: Next.js (App Router), PostgreSQL, Drizzle ORM, Tailwind CSS.

## Deploy for free (Vercel + Neon)

1. Create a free Postgres database at https://neon.tech and copy the connection string.
2. Create the tables (run once, from this folder):
   `DATABASE_URL="<your neon string>" npx drizzle-kit push`
   (If it uses `drizzle.config.json`, edit the `url` there temporarily to your Neon string.)
3. Push this project to GitHub.
4. At https://vercel.com choose **Add New > Project**, import the repo, and name it `aslbethel`.
5. Add the environment variable `DATABASE_URL` with your Neon connection string.
6. Click **Deploy**. Your site will be live at `aslbethel.vercel.app`.
7. Custom domain: Vercel project > **Settings > Domains** > add `aslbethel.us`, then add the DNS records it shows you at your registrar.

Jobs are seeded automatically on first page load.
