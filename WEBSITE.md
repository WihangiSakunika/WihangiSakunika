# Academic homepage

Lightweight HTML, CSS, and JavaScript. No build tools, packages, backend, or paid services are required. The GitHub profile `README.md` and existing images are unchanged.

## Deployment

The repository was already configured for **Settings → Pages → Deploy from a branch → main → / (root)** when inspected. Merge the website changes into `main` to trigger the existing Pages deployment. No repository settings change or custom workflow is needed. `.nojekyll` makes the root site serve as static files.

Expected URL: https://wihangisakunika.github.io/WihangiSakunika/

After merging, wait for the `pages-build-deployment` workflow to complete. Open the URL and confirm the portrait, styles, and navigation load. A hard refresh may be needed while cached Pages content expires.

If Pages is ever disabled, select the branch and folder above and save. Do not select `/docs` or GitHub Actions unless changing the deployment approach deliberately.

## Local preview

From the **parent directory** of this checkout, run:

```sh
python3 -m http.server 8000
```

If the checkout directory is named `WihangiSakunika`, visit `http://localhost:8000/WihangiSakunika/`. This checks the same subpath as production. No build step is needed. Keep asset paths relative to `index.html`.

## Editing

- `index.html`: biography, research interests, projects, education, experience, skills, contact, and SEO metadata.
- `assets/styles.css`: responsive sidebar, typography, colors, print styles, and reduced-motion support.
- `assets/main.js`: progressive mobile menu, section highlighting, and footer year. All page content and links remain available without JavaScript.
- `assets/images/wihangi-sakunika.jpg`: real GitHub avatar downloaded from https://avatars.githubusercontent.com/u/87114249?v=4.
- `assets/images/favicon.svg`: original WS monogram.

Update the local portrait when the GitHub avatar changes. The site does not depend on third-party fonts, scripts, or icon services.

## Content sources and decisions

The repository README was the primary source for biography, experience, research interests, skills, project descriptions, degree names, and study dates. The user supplied the WUT affiliation and contact links and confirmed that the Cardiff Metropolitan BSc and PIBT Advanced Diploma are completed. The user explicitly asked to omit the University of Kelaniya MIT from this website. WUT study remains ongoing (2026–present).

The layout takes structural inspiration from https://junwzhou.github.io/ (profile sidebar, top navigation, and academic sections). This is an original implementation; none of the professor's identity, achievements, publications, source code, or tracking scripts is included.

No verified publications or project-specific repository URLs were found in the README. The site uses the requested publications message and does not invent links or achievements. Project topic labels do not imply a technology stack beyond what the README supports. Research directions are described as interests, not completed outcomes. QA roles ended in August 2026 and are presented as past experience.

The correct LinkedIn URL in the README header and task brief is used. A malformed duplicate near the bottom of the README was not carried over. The README itself remains unchanged.

## Maintenance checks

Test at desktop, tablet, and mobile widths; check the menu with keyboard and touch; verify every anchor and local asset; check browser console errors and horizontal overflow. Keep external profile links at their verified addresses with `rel="noopener noreferrer"`. LinkedIn and Academia.edu may restrict automated visitors or require sign-in, so their destination content should be checked while signed in when necessary.
