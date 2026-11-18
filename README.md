# Stephen Chapman — personal research website

A static academic website, ready for GitHub Pages. It includes research themes, selected publications, teaching and scholarship, a short biography and contact information. No installation, package manager or build step is required.

## Open it on your computer

Unzip `Stephen_Chapman_Research_Website.zip`. Double-click `index.html` to open it in your browser. Keep `styles.css` and `favicon.svg` beside it.

## GitHub in plain English

Git is a system for tracking changes to files. GitHub is a website that stores Git projects and supports collaboration. GitHub Pages publishes website files from a GitHub repository.

| Term | What it means for this website |
| --- | --- |
| Repository, or repo | The project folder containing your website files and their history |
| Commit | A saved change with a message describing what you changed |
| Branch | A separate line of work; `main` will hold your published version |
| Clone | A local copy of a repository, including its Git history |
| Push | Sending your local commits to GitHub |
| Pull | Bringing changes from GitHub to your local copy |
| Pull request | A proposed change that can be reviewed before merging |
| GitHub Pages | The hosting service that turns your files into a live website |

You can begin entirely in your browser. Cloning, pushing and pulling become useful when you start editing locally or collaborating.

## Publish your first website

1. Sign in at https://github.com/ or create an account if you do not have one.
2. Create a new repository. For a personal website, name it **YOURUSERNAME.github.io**, replacing YOURUSERNAME with your exact GitHub username. This is an example pattern, not a username already selected for you.
3. Choose **Public** for the GitHub Free route and add a README so the repository has an initial branch. Your uploaded files and their history will be public, so upload only material you intend to share.
4. Open the repository's **Code** tab. Select **Add file → Upload files**.
5. Upload the extracted `index.html`, `styles.css`, `favicon.svg` and `student_map.html` files. Put them directly at the repository's top level. Upload the actual files, not the ZIP or a folder containing them. You may also upload this README to replace the initial one.
6. Enter a commit message such as `Add my research website` and commit to `main`.
7. Go to **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**. Select **main** and **/(root)**, then save.
8. Wait for the deployment. GitHub says publication can take up to ten minutes. The Pages settings will show the website address; the **Actions** tab shows deployment progress or errors.

Your personal website address follows the pattern `https://YOURUSERNAME.github.io/`.

The archive also includes an empty `.nojekyll` file. Upload it if it is visible in your file picker. It disables Jekyll processing; this simple site also works with GitHub Pages' default processing, so it is fine to begin with the four visible website files.

If you already have a personal website repository, create a separate repository such as `research-website` instead of overwriting it. A project website then follows the pattern `https://YOURUSERNAME.github.io/research-website/`. The relative asset links in this site support either arrangement.

## Make your first edit

Try changing the introductory sentence:

1. In your repository, open **index.html** and click the pencil icon to edit.
2. Find `I study how biological systems work` using your browser's Find command.
3. Edit the text between the `<p>` and `</p>` tags, leaving the tags in place.
4. Choose **Commit changes**, with a message such as `Update research introduction`.
5. Commit to `main`. Pages will redeploy; refresh the live site after it finishes.

For larger changes, create a branch, edit there, open a pull request and review it before merging into `main`. A branch alone does not create a separate live preview with this setup.

## Where to edit things

| What to change | Where to look |
| --- | --- |
| Name and browser-tab title | `<title>` and the header in `index.html` |
| Introductory text | Section with `id="home"` |
| Research themes | Section with `id="research"` |
| Papers, author lists and DOI links | Section with `id="publications"` |
| Teaching text | Section with `id="teaching"` |
| Biography | Section with `id="about"` |
| Email | Section with `id="contact"`; update both the displayed address and `mailto:` link |
| Colours | Variables at the beginning of `styles.css` |
| Layout and mobile behaviour | Rules in `styles.css` |
| Small browser-tab icon | `favicon.svg` |

To add a publication, copy one complete `<a class="paper" ...> ... </a>` block inside the publications section, then edit its year, journal, title, authors and DOI URL. A DOI link should start `https://doi.org/`.

You can later add links to public code repositories, an ORCID profile, teaching notebooks, a CV or project pages. No GitHub username, ORCID identifier, photograph or unpublished project details have been guessed for this version.

## Troubleshooting

- **A README appears instead of the website:** Check that `index.html` is at the top level of the branch/folder selected in Pages settings.
- **The website has no styling:** Check that `styles.css` is alongside `index.html`, with exactly that spelling and case.
- **A 404 appears:** Check the repository name, Pages source settings and deployment result in Actions. Allow the initial deployment to finish.
- **An edit does not appear:** Check the latest deployment and try refreshing the page without the browser cache.

## Content notes

This is an initial draft for your review. Professional details and selected publication metadata were checked against your University of Liverpool pages on 17 November 2026. The network graphic is an abstract illustration, not an experimental result or a specific metabolic pathway. This is a personal website, rather than an official University website. No analytics or contact-form backend are included. The Folium map loads external mapping assets as described below.

Sources for reviewing your content:

- Profile: https://www.liverpool.ac.uk/people/stephen-chapman
- Publications: https://www.liverpool.ac.uk/people/stephen-chapman/research-outputs
- Teaching: https://www.liverpool.ac.uk/people/stephen-chapman/teaching

Official GitHub guidance:

- https://docs.github.com/en/pages/quickstart
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site


## Supervision map and new sections

The website embeds `student_map.html`, the Folium export supplied on 17 November 2026. Upload it alongside `index.html`, `styles.css` and `favicon.svg`. The supplied marker locations and popup labels are preserved. To refresh the map later, export a new Folium HTML file with the same filename and replace that file in the repository.

The map requires internet access for Leaflet, supporting scripts/styles and OpenStreetMap tiles. These external services are used only by the embedded map; the rest of the site uses local assets.

Research history is in `id="research-history"`; supervision is in `id="supervision"`; personal interests are in `id="beyond-work"`. The map has a descriptive iframe title, a degree-level legend and a full-screen link.

GitHub profile checked on 17 November 2026: display name Stephen Chapman, username schapman6. The requested StephenChapman username was reported unavailable.


## Animated network graphic

The introductory illustration has travelling signals, gently pulsing node outlines and a slowly rotating dashed ring. A Pause/Play animation button controls all motion. The graphic remains static when the visitor has enabled reduced motion in their device settings. Animation uses inline SVG and CSS; the small inline script operates the pause control.


## Teaching image

The teaching section includes `assets/pymol-teaching.png`, an AI-generated illustrative scene based on reference photos supplied by Stephen Chapman. Its visible caption identifies it as generated. Upload the `assets` folder with the other website files so this image loads. Original reference photographs are not included in the website.


The generated teaching illustration has been removed at the owner’s request.
