# Meadow

Meadow is a single-file React + Supabase web app — a private community feed for members to post, ask for and offer help, and browse a member directory, with English/Persian (Farsi) language support.

## Structure

- `index.html` — the entire app (React 18 + Supabase JS, loaded via CDN, no build step required).

## Setup

1. Create a [Supabase](https://supabase.com) project with `members` and `posts` tables.
2. Open `index.html` and confirm `SUPABASE_URL` and `SUPABASE_ANON_KEY` near the top of the `<script>` block point to your project (Project Settings → API).
3. Serve `index.html` with any static host (or open it directly in a browser).

## Notes

This is a prototype: member passwords are stored in plain text in the `members` table, and the admin password is hardcoded in the client-side source. Do not reuse real passwords, and treat this as unsuitable for production use without hardening auth first.
