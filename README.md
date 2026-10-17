# The Book Detective Agency, website

Static site for thebookdetectiveagency.com. No build step. GitHub Pages serves the folder as is.

## Files
- index.html, the landing page. Styling is inline so the page matches the approved design one to one.
- styles.css, base rules and color tokens.
- research.html, the evidence page, twelve verified citations mapped to the rules of the game.
- story.html, the origin story and the maker's credentials. One bracketed paragraph waits for your own first-week account.
- teachers.html, classroom use, standards mapping for the four card colors, printing, licensing, pilot call.
- supplies.html, the storeroom: 22 Amazon affiliate links (four essentials, printing, desk, the eight authors' books), all rated 4.6 or higher in October 2026.
- assets/, the character images and the social preview image.
- CNAME, the custom domain for GitHub Pages. Do not rename.
- robots.txt, sitemap.xml, .nojekyll.

## Deploy
1. Create a public repository on GitHub, for example `thebookdetectiveagency`.
2. Upload every file in this folder to the repository root.
3. Settings, Pages, Source: Deploy from a branch, branch `main`, folder `/ (root)`.
4. Settings, Pages, Custom domain: enter thebookdetectiveagency.com and save. Tick Enforce HTTPS once the certificate appears, which takes up to an hour.

## DNS at the registrar
Add these records where you bought the domain.

A records for the apex (@), all four:
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

CNAME record for www pointing to `YOUR-GITHUB-USERNAME.github.io`

Propagation takes minutes to a day. Verify with https://dnschecker.org.

## Before launch
- Replace `YOUR-STORE.lemonsqueezy.com/checkout/buy/PRODUCT-ID` with the real checkout link.
- Replace `[YOUR-TAG]` with the Associates tag in every file at once: `sed -i 's/\[YOUR-TAG\]/yourtag-20/g' index.html supplies.html`
- Put the binder photograph in assets/ and swap the placeholder box in the kit section for it.
- Fill the bracketed paragraph on story.html and swap the photograph placeholder for a real one in assets/.
- Set up hello@thebookdetectiveagency.com (Google Workspace or the registrar's email forwarding).

## Colors and type
Teal 1F5F68, Red C8402B, Gold B8780F, Violet 5B4A8A, Ink 1C1A16, Cream F6F3EC. Lexend throughout.
