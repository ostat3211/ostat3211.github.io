# Tom Ostapchuk's website

A static personal website using HTML and CSS. No packages or build step.

## Preview locally

Open `index.html` in a browser, or run this command from the project folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Visit <http://127.0.0.1:8000>. Press Control-C in the terminal to stop the server.

## Files

- `index.html`: page content and structure.
- `styles.css`: colours, typography, layout, and mobile styles.
- `assets/`: favicon and future images or résumé files.
- `.nojekyll`: tells GitHub Pages to serve the static files directly.

Use relative asset links such as `./styles.css` so the site works on both a GitHub project URL and a custom domain.

## Publish with GitHub Pages

1. Create a public GitHub repository. For an account homepage, name it `YOUR-USERNAME.github.io`. A project repository such as `tom-website` also works.
2. Push these files to its `main` branch.
3. In the repository, open **Settings > Pages**.
4. Select **Deploy from a branch**, choose **main** and **/ (root)**, then save.
5. Wait for the Pages deployment to finish. Open the URL shown in Settings.

Future pushes to `main` publish automatically. No custom GitHub Actions workflow is required.

GitHub Free requires a public repository for Pages. See [GitHub's setup guide](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Connect tomostapchuk.com when ready

The domain is not configured by this scaffold. First get the GitHub Pages URL working.

1. Verify domain ownership in GitHub's account settings.
2. Add `tomostapchuk.com` under the repository's **Settings > Pages > Custom domain**.
3. Follow [GitHub's current DNS instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) at the existing DNS provider. Preserve existing email records.
4. Enable **Enforce HTTPS** once the certificate is available.

GitHub creates the `CNAME` file when the custom domain is saved for branch publishing. Pull that change into the local repository before making further changes.

## Before the full launch

Replace the placeholder content with approved copy and links. Remove the `noindex, nofollow` robots meta tag from `index.html` when ready for search engines. Check the site on desktop and mobile, test keyboard navigation, and confirm every link.
