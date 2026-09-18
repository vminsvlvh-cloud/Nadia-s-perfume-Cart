NADIA'S PERFUME CART V23 — ADMIN READY

Built:
- admin.html login/dashboard
- Supabase-backed public announcement
- Arabic + English announcement text
- Link + show/hide
- Secure Row Level Security SQL
- Existing V22 local announcement remains as fallback until Supabase is configured

TO CONNECT:
1. Create a Supabase project.
2. In Supabase SQL Editor, run supabase-setup.sql.
3. Create the owner's user in Supabase Authentication.
4. Mark ONLY that user as admin using app_metadata.role = admin from a trusted admin/server context.
5. Put Project URL + Publishable/Anon key in supabase-config.js.
6. Upload V23 to GitHub; Railway redeploys automatically.
7. Open /admin.html and sign in.

SECURITY:
Never put the Supabase service_role/secret key in HTML/JavaScript/GitHub.
The frontend uses only the publishable/anon key and RLS protects writes.
