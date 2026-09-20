# SEA Trade website

A simple, self-contained website: `index.html`, `style.css`, `script.js`.
No build step, no dependencies to install — it works as plain files.

## 1. Before you publish: things to fill in

Open `index.html` in any text editor and change these (search for them):

| What | Where | Find this |
|---|---|---|
| WhatsApp number | appears twice | `https://wa.me/20000000000` — replace `20000000000` with your number in international format, no `+` or spaces (e.g. `201001234567`) |
| Phone number shown in text | inquiry section | `+20 000 000 0000` |
| Inquiry form | inquiry section | `https://formspree.io/f/YOUR_FORM_ID` — see step 2 below |

## 2. Make the inquiry form actually send you emails

The form needs somewhere to send its data, since a GitHub Pages site has no
server of its own. The easiest free option is **Formspree**:

1. Go to [formspree.io](https://formspree.io) and create a free account.
2. Create a new form. It will give you a URL like `https://formspree.io/f/abcdwxyz`.
3. In `index.html`, find this line:
   ```html
   <form class="inquiry-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
   Replace `YOUR_FORM_ID` with the code Formspree gave you.
4. Save, publish (steps below), then submit the form once yourself to confirm
   your email with Formspree — it will ask you to do this the first time.

That's it. Submissions will now arrive in your inbox. The free plan covers a
generous number of submissions per month, which is plenty for an inquiry form.

## 3. Publish it with GitHub Pages (free hosting)

1. Create a new repository on GitHub (e.g. `sea-trade-site`). Keep it Public.
2. Upload these three files to the repository: `index.html`, `style.css`, `script.js`.
   (On GitHub.com: **Add file → Upload files**, drag them in, then **Commit changes**.)
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. Wait a minute or two, then refresh the page — GitHub will show your live
   link, something like:
   ```
   https://YOUR-USERNAME.github.io/sea-trade-site/
   ```

That link is your website. Share it, put it on a business card, link to it
from WhatsApp Business — it works exactly like any other website.

## 4. Using your own domain (optional)

If you buy a domain (e.g. `seatrade.com`) later:

1. In the repository, go to **Settings → Pages → Custom domain** and type
   your domain in.
2. At your domain registrar, add a `CNAME` record pointing to
   `YOUR-USERNAME.github.io`.
3. GitHub will create a `CNAME` file in the repository automatically —
   leave it there.

This step is optional. The plain `github.io` link works fine on its own.

## 5. Making changes later

Edit `index.html` directly on GitHub (click the pencil icon on the file),
or download the files, edit them, and re-upload. Any commit to the `main`
branch updates the live site automatically within a minute or two.

## What's in each file

- **index.html** — all the page content and structure
- **style.css** — all colors, fonts, and layout
- **script.js** — the mobile menu, the footer year, and the FAQ accordion behavior

No other files are required. Everything (fonts included) loads from a CDN,
so there's nothing else to install or configure.
