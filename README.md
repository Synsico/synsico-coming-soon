# SYNSICO ANALYTICS - Coming Soon

A temporary, responsive landing page for SYNSICO ANALYTICS while the full website is being built.

**Tagline:** Systems for a Smarter World.

## What is included

- `index.html`: The complete page, including styles, JavaScript, logo artwork, and browser icon.
- `.nojekyll`: Tells GitHub Pages not to process the site as a Jekyll project.
- `.gitignore`: Excludes common local files and environment files from Git.
- `README.md`: This guide.

No installation, package manager, build command, external font, or image service is required. The page includes no forms, analytics, cookies, API keys, payment flow, or backend. The optional email link opens the visitor's email application; it does not submit or store data on this site.

The website itself is not deployed by downloading these files.

## Preview on your computer

Extract the ZIP, then double-click `index.html` to open it in your browser. Keep its filename as `index.html` when publishing.

## Publish using GitHub Pages

1. Create a repository in your GitHub account. Suggested name: `synsico-coming-soon`. On GitHub Free, the repository must be public for Pages.
2. Upload the extracted files to the root of the repository, not the ZIP itself. `index.html` must be visible directly in the repository's main file listing, not inside another folder. Include `.nojekyll`; your computer may hide files starting with a dot.
3. Commit the files to the `main` branch.
4. Open **Settings > Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Select **main** and **/(root)**, then choose **Save**.
5. After deployment finishes, return to **Settings > Pages** and open the published site URL. Check the deployment workflow if it reports an error.

For a normal GitHub.com project repository, the expected URL pattern is:

```text
https://YOUR-GITHUB-USERNAME.github.io/synsico-coming-soon/
```

`YOUR-GITHUB-USERNAME` is a placeholder, not a configured account. A custom domain and DNS are not configured in this package.

Official documentation, checked September 23, 2026:

- Creating a site: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- Publishing source: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- Project URL pattern: https://docs.github.com/en/get-started/start-your-journey/deploying-your-website-automatically

### Hosting policy

This is a non-transactional coming-soon page. GitHub Pages documentation restricts using Pages as free hosting to run an online business, facilitate commercial transactions, or provide commercial SaaS. The absence of checkout does not itself guarantee that a business site is permitted. Review GitHub's terms for your actual use. These static files are portable to another web host, and the code can remain in a GitHub repository even when the website is hosted elsewhere.

- GitHub Pages limits: https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits

Do not put passwords, private customer information, API keys, or confidential business plans into the repository. A private repository does not necessarily make its published Pages website private.

## Add your real business email

In `index.html`, find this near the bottom:

```javascript
const SITE_CONFIG = Object.freeze({
  contactEmail: ""
});
```

Put your confirmed public business email between the empty quotes. A valid address makes the **Contact us** link appear. Leaving it empty keeps the link hidden. No email address has been guessed or prefilled.

This is a `mailto:` link, not a hosted contact form or mailing-list subscription. To receive form submissions later, add a properly configured form service or backend and update the site's privacy information.

## Edit text and appearance

- Main heading: find `id="hero-title"`.
- Coming-soon description: find `class="intro"`.
- About panel: find `id="about-dialog"`.
- Business address: find `class="address"`.
- Theme colors: edit the CSS variables under `:root`.
- Page title and social sharing text: edit the `<title>` and `<meta>` tags near the top.

The supplied business address is labeled **Business address**, not a staffed office. No legal corporate suffix, public launch date, pricing, client results, partner endorsements, or certifications are asserted. Confirm that all copy and the supplied address are appropriate for public use before publishing.

The logo is embedded from the supplied SYNSICO artwork. You do not need to upload a separate logo image. Replace it with an approved high-resolution brand asset when available. No separate font files are included.

## Accessibility and privacy behavior

- Responsive desktop, tablet, and mobile layout.
- Visible keyboard focus and a skip-to-content link.
- The Discover Synsico dialog supports Escape, close-button dismissal, and focus return.
- Decorative motion has a pause control and honors reduced-motion preferences.
- Core content remains visible with JavaScript disabled, and decorative motion stays paused.
- No third-party requests are needed by the page code. A hosting provider may still maintain ordinary hosting/access logs.

## Validation performed

Tested in headless Chromium at widths of 320, 375, 390, 520, 768, 820, 1024, 1440, and 1920 pixels. No horizontal page overflow or JavaScript errors were found in those checks. The dialog, focus return, motion toggle, default hidden contact link, and JavaScript-disabled main content were also checked. Desktop and mobile screenshots were visually reviewed.

This is not a complete cross-browser, accessibility, legal, or security certification. Verify the actual deployed page on your own devices before announcing it.

## Replace this page later

Replace `index.html` with the full site's entry page and upload its assets. A full site's hosting and build requirements may differ from this standalone placeholder. Remove outdated coming-soon text and update metadata when you launch.
