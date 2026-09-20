# Mutagarat website

A simple, self-contained website: `index.html`, `style.css`, `script.js`.
No build step, no dependencies to install, it works as plain files.

## 1. Already filled in

These are already set for you, no editing needed:

| What | Value |
|---|---|
| WhatsApp number | `+20 127 960 0002` (used in the header and the inquiry section) |
| Inquiry form | Connected to Formspree (`https://formspree.io/f/moevevab`) |

The one thing left to do before the form actually delivers to your inbox:
submit it once yourself after publishing, since Formspree asks you to confirm
your email the first time a submission comes through. After that, every
submission arrives in whatever inbox you used to sign up at formspree.io. The
free plan covers a generous number of submissions per month, plenty for an
inquiry form.

## 2. Publish it with GitHub Pages (free hosting)

1. Create a new repository on GitHub (e.g. `mutagarat-site`). Keep it Public.
2. Upload these three files to the repository: `index.html`, `style.css`, `script.js`.
   (On GitHub.com: **Add file → Upload files**, drag them in, then **Commit changes**.)
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. Wait a minute or two, then refresh the page. GitHub will show your live
   link, something like:
   ```
   https://YOUR-USERNAME.github.io/mutagarat-site/
   ```
7. Submit the inquiry form on the live site once yourself, so Formspree can
   confirm your email and start forwarding submissions.

That link is your website. Share it, put it on a business card, link to it
from WhatsApp Business, it works exactly like any other website.

## 3. Using your own domain (optional)

If you buy a domain later:

1. In the repository, go to **Settings → Pages → Custom domain** and type
   your domain in.
2. At your domain registrar, add a `CNAME` record pointing to
   `YOUR-USERNAME.github.io`.
3. GitHub will create a `CNAME` file in the repository automatically, leave
   it there.

This step is optional. The plain `github.io` link works fine on its own.

## 4. Making changes later

Edit `index.html` directly on GitHub (click the pencil icon on the file),
or download the files, edit them, and re-upload. Any commit to the `main`
branch updates the live site automatically within a minute or two.

## What's in each file

- **index.html**: all the page content and structure
- **style.css**: all colors, fonts, and layout
- **script.js**: the mobile menu, the footer year, and the FAQ accordion behavior

No other files are required. Everything (fonts included) loads from a CDN,
so there's nothing else to install or configure.
