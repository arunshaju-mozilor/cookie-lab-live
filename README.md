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

`index.html` loads the Live banner in `<head>`:

```html
<script id="cookieyes" type="text/javascript"
  src="https://cdn-cookieyes.com/client_data/2a580c28b7926400613c8dfd31c73acf/script.js">
</script>
```

The other pages have no CookieYes script installed.

## Hosting

GitHub Pages: **Deploy from a branch → `main` → `/` (root)**.
Pushing to `main` redeploys the site within a minute or two.

Use https://arunshaju-mozilor.github.io/cookie-lab-live/ as the domain when adding the website
in the CookieYes dashboard.
