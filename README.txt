Mind Maps (iPad app)

INSTALL
1. Host this folder on any static HTTPS site (GitHub Pages: put the files at the top level of a repo,
   Settings > Pages > Deploy from branch main / root. Or drag the folder onto Netlify Drop).
2. On the iPad open the site in Safari > Share > Add to Home Screen.
Updating: replace the files. If the installed app looks stale, close and reopen it once or twice
(bump the cache name V in sw.js when you change files).

SIGN-IN AND SYNC (optional, free)
Sign-in uses a Supabase project that you own, so your maps live in your own account.
1. Create a free project at supabase.com.
2. In the project: SQL Editor > paste the SQL from the app (Account sheet > Copy setup SQL) > Run.
3. Project Settings > API: copy the Project URL and the anon public key.
4. In the app: Account button > paste URL and anon key > Save, then Create account / Sign in.
   (Or put the URL and key in config.js before hosting, so the app is pre-connected.)
Auth > Providers > Email: turn "Confirm email" off if you want to sign in right after creating an account.
The anon key is designed to be public. Row-level security in the SQL keeps each person's rows private.

AI IMPORT
Settings > paste an Anthropic API key. After you pick a .pptx a sheet asks how the map should be organized.
The key stays on the device and is sent only to api.anthropic.com.
