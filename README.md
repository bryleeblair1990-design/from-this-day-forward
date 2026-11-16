# From This Day Forward

A small shared web app for two people to work through five relationship commitments together.

## Included
- Sign-up/sign-in using Supabase Auth
- Create a couple space and invite one partner with a code
- Shared checklist progress with realtime refresh
- Shared journal entries
- Five commitments and 30 daily booster prompts, adapted from the participant guide

## Setup
1. Create a Supabase project at https://supabase.com.
2. Open **SQL Editor**, paste `supabase_setup.sql`, and run it.
3. In **Project Settings > API**, copy the Project URL and the publishable/anon key.
4. Open `index.html` in a browser for local testing, enter those two public settings, and create an account.
5. For a shareable website, deploy this folder to a static host such as Vercel or Netlify. Add your site's URL to Supabase Auth's allowed redirect/site URL settings if needed.
6. Create a space, then send the invite code to your partner. They create their own account and join with that code.

## Important
- Never put a Supabase service-role key or database password in the browser.
- The invite code is a one-time join code; only share it with the intended partner.
- The app currently saves commitment checklist progress and journal entries in the shared database. The 30-day booster checkboxes are currently local to the browser and do not sync yet.
- This is a starter version, not a substitute for professional relationship or pastoral counseling.
- The source guide's engaged-couple assessment is not included in this starter build; this app is intended for a dating couple preparing thoughtfully for the future.
