# Setting up your website

Your site has three parts, all free:

| Part | What it does | Where |
|---|---|---|
| **Website** | The public page | `ruchii-prasad.github.io` |
| **Admin panel** | Add or edit projects, achievements and papers, and upload PDFs, from a form | `ruchii-prasad.github.io/admin` |
| **Contact form + analytics** | Messages from visitors land in your inbox, and you can see who visits and which papers get opened | Web3Forms + GoatCounter |

## How it works

- All your content lives in the `content/` folder as data files.
- The admin panel edits those files for you and saves each change straight to your GitHub repo.
- GitHub Pages republishes the site automatically, usually within 1–2 minutes.
- Uploaded PDFs, like papers and your résumé, go into the `uploads/` folder.

There is no server to run or pay for.

---

## 1. Publish the site (one time)

1. Create a **public** repo named exactly `ruchii-prasad.github.io`.
2. Unzip `website.zip`. Upload **everything inside it**, including the `admin`, `content` and `uploads` folders and the `.nojekyll` file, using Add file → Upload files. Dragging the folders in works.
3. Go to **Settings → Pages**. Set Source to *Deploy from a branch*, Branch to `main`, and folder to `/ (root)`.
4. After 1–2 minutes the site is live at **https://ruchii-prasad.github.io**.

## 2. Set up the admin panel (one time)

The admin panel signs in with a GitHub access token. The token lets it save changes to your repo, and only to that repo.

1. Open GitHub → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. **Repository access:** choose *Only select repositories*, then pick `ruchii-prasad.github.io`.
3. **Permissions → Repository permissions → Contents:** set to *Read and write*.
4. Pick an expiry (up to 1 year), generate the token, and copy it.
5. Go to **https://ruchii-prasad.github.io/admin**, click **Sign In with Token**, and paste it.

The token is stored only in that browser. Treat it like a password. Don't share it, and don't paste it anywhere else. When it expires, generate a new one the same way.

## 3. Turn on the contact form (optional)

1. Go to **web3forms.com** and enter the email address where you want to receive messages. They'll email you an **access key**.
2. In the admin panel, open **Settings** and paste the key into *Contact form access key*. Save.

The form appears in the Contact section. The free plan allows 250 messages a month. The access key is designed to be public, so it's fine for it to sit in your site's files.

## 4. Turn on analytics (optional)

1. Sign up at **goatcounter.com** (free for personal sites) and choose a code, for example `ruchiprasad` → `ruchiprasad.goatcounter.com`.
2. In the admin panel, open **Settings** and enter just the code (`ruchiprasad`). Save.
3. Your GoatCounter dashboard then shows page views, where visitors come from, and events like:
   - `pdf-<paper-name>`: someone opened one of your papers
   - `resume`: someone opened your résumé
   - `contact-form-sent`: someone messaged you

---

## Everyday use

- **Add a project, achievement or paper:** go to `/admin`, open the section, click **Add**, fill in the form, and click **Save**. The site updates in 1–2 minutes.
- **Publish a paper:** in *Research papers*, add a paper and use the **Paper PDF** field to upload the file. The site adds the PDF link, the abstract toggle, and the Cite button for you.
- **Reorder items:** drag them in the list. The order in the admin panel is the order on the site.
- **Empty sections stay hidden.** Achievements, Research and Experience appear on the site, and in the top menu, only once they have at least one entry.

## Before you go live

In the admin panel, open **Profile & links** and:
- Replace `YOUR_EMAIL@example.com` with your email.
- Upload your résumé to show the Résumé button.
