# Cookie Lab — Live

A minimal static site for CookieYes banner QA testing against the **Live** environment.
Dark violet theme; every page shows a `Live` tag in the nav.

**Live:** https://arunshaju-mozilor.github.io/cookie-lab-live/

## Pages

| Page | Purpose |
|---|---|
| `index.html` | **Cookie Lab** home page — loads real third-party trackers and sets cookies in every category on load, with a live consent-status dashboard |
| `about.html` | About page for multi-page navigation tests |
| `privacy-policy.html` | Privacy policy (linked from banner) |
| `cookie-policy.html` | Cookie policy page (no CookieYes policy script installed) |
| `terms-and-conditions.html` | Terms and Conditions page — heading only, blank body |

## CookieYes script

No CookieYes script is installed. To test a banner, add the account's `<script id="cookieyes" ...>`
tag to the `<head>` of each page (and the cookie-policy script to `cookie-policy.html`).

## Hosting

GitHub Pages: **Deploy from a branch → `main` → `/` (root)**.
Pushing to `main` redeploys the site within a minute or two.

Use https://arunshaju-mozilor.github.io/cookie-lab-live/ as the domain when adding the website
in the CookieYes dashboard.
