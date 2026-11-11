ORBIT ATLAS: how to put it online
=================================
Files: index.html (landing page), tracker.html (the app), favicon.svg, robots.txt.
No build step, no server code. It is a static site.

Easiest options (all free):
1. Netlify Drop: go to app.netlify.com/drop and drag this folder in. You get a link in seconds.
2. Cloudflare Pages or GitHub Pages: upload the files, publish, done.
3. Normal web hosting: upload everything into public_html with the file manager or FTP.

Notes
- The tracker loads live orbit data from CelesTrak (celestrak.org) in each visitor's browser and caches it for 2 hours. Please keep that cache; CelesTrak asks apps not to refetch more often.
- It uses satellite.js from the jsDelivr CDN. To self-host, download satellite.min.js and change the script tag in tracker.html.
- Add your own domain, a sitemap.xml and social preview tags once you know the final address.
