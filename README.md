# sayanchk-website

Personal website for [Sayan Chakraborty](https://sayanch.com), migrated from WordPress to a static multi-page HTML site hosted on GitHub Pages.

## Site Structure

| File | Page |
|------|------|
| `index.html` | Home — Bio |
| `experiences.html` | Work experience |
| `publications.html` | Research publications |
| `patents.html` | US Patents |
| `softwares.html` | Open-source software (Luminaire) |
| `conference-talks.html` | Conference presentations |
| `media.html` | Media appearances |
| `blog.html` | Blog |
| `css/style.css` | Shared styles (light/dark theme) |
| `js/main.js` | Theme toggle & nav behavior |

## Activating GitHub Pages

1. Push all files to the `main` branch of this repo.
2. Go to **Settings → Pages** in the GitHub repository.
3. Under **Source**, select **Deploy from a branch**.
4. Choose branch `main` and folder `/ (root)`, then click **Save**.
5. After a minute or two, the site will be live at:

   ```
   https://sayanchakraborty.github.io/sayanchk-website/
   ```

## Local Preview

Open `index.html` directly in a browser, or run a local server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Customization Notes

- **LinkedIn URL**: The nav LinkedIn link points to `https://www.linkedin.com/in/sayanchakraborty/`. Update this in each HTML file's `<nav>` block if your profile URL is different.
- **Logo**: The SC logo is loaded from the WordPress CDN. Download it and place it locally (e.g. `assets/logo.png`) to remove the dependency on `sayanch.com`.
- **Dark/Light Mode**: Preference is saved in `localStorage` under the key `sc-theme` and defaults to the OS preference.
