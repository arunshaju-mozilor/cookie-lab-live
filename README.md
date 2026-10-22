# Cookie Lab — QA1 Basic

A minimal static site for CookieYes banner QA testing against the **QA1** environment,
wired to a **Basic-plan** site. Dark violet theme; every page shows a `QA1 · Basic` tag in the nav.

**Live:** https://arunshaju-mozilor.github.io/cookie-lab-qa1-basic/

## Pages

| Page | Purpose |
|---|---|
| `index.html` | **Cookie Lab** home page — loads real third-party trackers and sets cookies in every category on load, with a live consent-status dashboard |
| `about.html` | About page for multi-page navigation tests |
| `privacy-policy.html` | Privacy policy (linked from banner) |
| `cookie-policy.html` | Renders the CookieYes cookie policy for the same QA1 account |
| `terms-and-conditions.html` | Terms and Conditions page — heading only, blank body |

## CookieYes script

Every page loads the QA1 Basic banner in `<head>`:

```html
<script id="cookieyes" type="text/javascript"
  src="https://cdn-mojoview.uk/client_data/3ff46f3c60ae20a91dd55a0cce554982/script.js">
</script>
```

`cookie-policy.html` also loads `.../client_data/3ff46f3c60ae20a91dd55a0cce554982/cookie-policy/script.js`.
To switch accounts, replace the client ID in all four HTML files.

## Hosting

GitHub Pages: **Deploy from a branch → `main` → `/` (root)**.
Pushing to `main` redeploys the site within a minute or two.

Use https://arunshaju-mozilor.github.io/cookie-lab-qa1-basic/ as the domain when adding the website
in the QA1 CookieYes dashboard.
