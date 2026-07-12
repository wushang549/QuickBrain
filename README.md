# QuickMind Games

Static marketing website for the iOS app QuickMind Games.

## Run locally

This site is plain HTML, CSS, and JavaScript. From the project root, run:

```bash
python -m http.server 8080
```

Then open:

```text
http://localhost:8080/
```

## Routes

- `/`
- `/privacy/`
- `/support/`
- `/terms/`
- `/app-ads.txt`

The `app-ads.txt` file is located at the project root so it can be served exactly from `/app-ads.txt`.

## Deploy

Deploy the full folder to any static hosting provider, such as Netlify, Vercel static output, Cloudflare Pages, Firebase Hosting, or GitHub Pages with a custom domain. Make sure the host preserves root files and directory index files.

## Change domain or email

The current contact email placeholder is:

```text
quickbraindev@gmail.com
```

Search for that value in the HTML files and replace it with the real support email. Update any hosting or DNS settings in your static host when connecting the final custom domain.

## Images

The landing page uses the app logo from:

```text
imagenes/logo.png
```

The screenshot showcase uses mockups from:

```text
imagenes/edits/
```

## StoreKit product ID note

The current app code may use this product ID:

```text
quickmind.removeads.lifetime
```

Before creating the real product in App Store Connect, consider updating it to a final-name-aligned value such as:

```text
quickbrain.removeads.lifetime
```

Do not change this automatically unless the app code has a clearly isolated StoreKit product ID definition. If the iOS code depends on the old ID, update every StoreKit product reference, purchase lookup, restore path, entitlement check, and any App Store Connect product configuration together.
