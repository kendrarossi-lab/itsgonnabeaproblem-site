# It's Gonna Be a Problem (itsgonnabeaproblem.com) - DRAFT site

This is a draft static website for Kendra Jade's relationships podcast It's Gonna Be a Problem. It is not published.

Do not deploy, point DNS, submit sitemaps, pay for hosting, or announce the site until Kendra gives a direct OK.

## What's in this folder

Plain HTML and CSS. No build step. Open it with any static host, or locally with a simple server (paths are root-absolute, so opening files with a file:// URL will break CSS).

Suggested local preview:

    python3 -m http.server 8080 --directory .

Then visit http://127.0.0.1:8080/

## Pages

- `/` Home: cover, show pitch, launch date (Tuesday, December 1, 2026), placeholder listen buttons, Season 1 launch episodes, story CTA, socials
- `/episodes/` Season 1 launch archive (trailer plus Episodes 1 to 3)
- `/episodes/trailer/`
- `/episodes/dating-standards-why-im-done-being-easy/`
- `/episodes/red-flags-in-dating-i-used-to-call-cute/`
- `/episodes/situationships-are-a-problem/`
- `/about/` Host and show, house rules, explicit rating
- `/stories/` mailto stories@ plus what-to-send guide and privacy promise
- `/contact/` hello@, booking@, stories@, socials
- `/shop/` Show merch coming soon (no products or prices yet)
- `/listen/` Coming Dec 1 placeholders for Spotify, Apple Podcasts, and Amazon Music
- `/404.html` Custom not-found page pointing back to episodes and listen

SEO is included: unique titles and meta descriptions, Open Graph and Twitter card image, favicon, PodcastSeries and PodcastEpisode JSON-LD, sitemap.xml, robots.txt, canonical URLs for https://itsgonnabeaproblem.com, and a CNAME file containing itsgonnabeaproblem.com.

Listen buttons are not live links. The Spotify show is still unpublished.

## Recommended host

GitHub Pages (free, custom domain supported). Kendra already has a GitHub account signed in with Google at kendrarossi@gmail.com. The GitHub username is not recorded in the current Accounts and Logins file, so the www CNAME target should be filled in as `<github-username>.github.io` once the username or organization is confirmed.

Do not reuse a Cloudflare Pages account that already hosts a different project. If Cloudflare Pages is preferred later, create a new account for this show (for example with itsgonnabeaproblem@gmail.com or kendrarossi@gmail.com) after Kendra OKs it.

## DNS records for GitHub Pages (hand these to Domains Bot after Kendra OKs hosting)

Root (apex) `itsgonnabeaproblem.com`, type A, four records:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

Optional IPv6 AAAA records:

- 2606:50c0:8000::153
- 2606:50c0:8001::153
- 2606:50c0:8002::153
- 2606:50c0:8003::153

`www` CNAME: `<github-username>.github.io`

Also set the custom domain to itsgonnabeaproblem.com in the GitHub repo Pages settings, and keep the CNAME file in this folder. A `.nojekyll` file is included so GitHub Pages will not run Jekyll.

If Cloudflare Pages is used instead (new account only):

- Root `@` CNAME (flattened by Cloudflare) to `<project>.pages.dev`
- `www` CNAME to `<project>.pages.dev`

## After Kendra OKs publish

1. Create a public GitHub repo (for example `itsgonnabeaproblem` or `itsgonnabeaproblem.github.io`) under the existing account.
2. Upload these files to the default branch.
3. Enable GitHub Pages from the branch root.
4. Ask Domains Bot to add the A and CNAME records above.
5. Swap placeholder listen buttons for real Spotify, Apple Podcasts, and Amazon Music URLs once those are live.
6. Do not spend money or email anyone from this folder.

Copy on this site comes from the show SEO pack, Season 1 show notes, story submission setup, and show-level descriptions. Episode writing remains paused except for using existing approved draft copy already on the page.
