# It's Gonna Be a Problem (itsgonnabeaproblem.com)

Static website for Kendra Jade's relationships podcast It's Gonna Be a Problem.

The public site is hosted on GitHub Pages from the `kendrarossi-lab/itsgonnabeaproblem-site` repo, custom domain `itsgonnabeaproblem.com`, serving from the `main` branch root. The CNAME file in this folder must stay set to `itsgonnabeaproblem.com`. A `.nojekyll` file is included so GitHub Pages will not run Jekyll.

Plain HTML and CSS. No build step. Paths are root-absolute, so opening files with a file:// URL will break CSS.

Suggested local preview:

    python3 -m http.server 8080 --directory .

Then visit http://127.0.0.1:8080/

## Pages

- `/` Home: cover, official pinstripe title card, show pitch, launch date (Tuesday, December 1, 2026), placeholder listen buttons, Season 1 launch episodes (trailer plus Episodes 1 to 3), story CTA, socials, FAQ teaser, launch-reminder mailto
- `/episodes/` Season 1 launch archive (trailer plus Episodes 1 to 3)
- `/episodes/trailer/`
- `/episodes/dating-standards-why-im-done-being-easy/`
- `/episodes/red-flags-in-dating-i-used-to-call-cute/`
- `/episodes/situationships-are-a-problem/`
- `/about/` Host and show, house rules, explicit rating, official promo photos
- `/stories/` mailto stories@ plus what-to-send guide and privacy promise
- `/contact/` hello@, booking@, stories@, socials, launch-reminder mailto
- `/shop/` Show merch coming soon (no products or prices yet)
- `/listen/` Coming Dec 1 placeholders for Spotify, Apple Podcasts, Amazon Music, and YouTube, plus a YouTube embed placeholder and the official channel link
- `/faq/` Launch, listen, stories, and show FAQ
- `/404.html` Custom not-found page pointing back to episodes and listen

SEO includes unique titles and meta descriptions, Open Graph and Twitter cards, favicon and web manifest, WebSite, PodcastSeries, Person, and PodcastEpisode JSON-LD, FAQPage schema, sitemap.xml, robots.txt, and canonical URLs for https://itsgonnabeaproblem.com.

Listen buttons are not live links until the show publishes on Tuesday, December 1, 2026. The Spotify show (id 3JfiJQ799cpEyo8e22Sl8A) is still unpublished. Do not add fake play buttons.

Styles: edit `css/styles.css`, then regenerate `css/styles.min.css` (the file pages actually load).

## DNS and HTTPS notes

Porkbun DNS for the apex (A and AAAA to GitHub Pages) and `www` CNAME to `kendrarossi-lab.github.io` is already in place. If browsers show a certificate error on https://www.itsgonnabeaproblem.com or https://itsgonnabeaproblem.com, GitHub Pages still needs a custom-domain certificate. That is fixed in the repo's GitHub Pages settings (custom domain `itsgonnabeaproblem.com`, then Enforce HTTPS). Do not change the Porkbun records for that step unless Pages says the `www` CNAME is wrong.

Google Search Console for the domain is handled separately. Do not add verification tags in these files unless asked.

## Photo rule for this repo

The official image set, as of November 24, 2026, is the four files Kendra sent that day: three title cards (pinstripe seated, director chair reclining, cape standing) and the Queen Kendra logo. Use them as is. Do not retouch. Do not remove tattoos or change clothing. Only resized, cropped-for-format, and webp copies belong in `/images`. The Rain Check cover stays as the podcast cover art.

## Publishing

The box cannot `git push`. New or changed files are uploaded through the GitHub web UI to `main`, then Pages rebuilds. Nothing else should be submitted, emailed, or paid for from this folder without Kendra's own-words OK.
