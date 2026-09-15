# Michal Merav — personal website

This folder is a small website. A website is just files. A browser reads those files and draws a page.

You do not need to install anything extra to edit it. You open a file, change some words, save, and look at the page again.

The live address (after you publish) will be:

https://michellemerav.github.io

That address only works if your GitHub username is `michellemerav` and the GitHub project is named exactly `michellemerav.github.io`. The folder on your computer can stay named `website_test1`.

---

## What each file is

Think of HTML files as **the pages** (the words and pictures) and CSS as **the look** (colors and layout).

| File | What it is |
| --- | --- |
| `index.html` | Home / summary. The first page people see. Keep this file name. |
| `art.html` | Art portfolio |
| `projects.html` | Engineering projects |
| `resume.html` | Resume / CV |
| `publications.html` | Papers + Google Scholar link |
| `css/style.css` | Colors, fonts, spacing. One change here updates every page. |
| `images/art/` | Put art photos here later |
| `images/projects/` | Put project photos here later (optional) |
| `files/` | Put `resume.pdf` here later |

Google Scholar and LinkedIn are already filled in on every page.

---

## How to look at the site on your computer

1. Open this folder in File Explorer.
2. Double-click `index.html`.
3. It should open in your browser (Chrome, Edge, etc.).
4. Click the menu words at the top to move between pages.

If a page looks wrong after you edit, save the file and click Refresh.

---

## How to change text

1. Open the page file (for example `index.html`) in any text editor. Cursor, Notepad, or GitHub Desktop’s editor all work.
2. Look for comments. Comments look like this and do **not** show on the website:

   `<!-- this is a note to you -->`

3. Change only the words between the tags, for example the sentence inside `<p> ... </p>`.
4. Save. Refresh the browser.

Do not delete the `<` `>` tags around the words. Those tell the browser what each piece is.

**Name at the top:** it is written once in each HTML file, next to `class="site-name"`. If you change the name, change it in all five HTML files, and in the `<title>` line near the top of each file.

**Colors:** open `css/style.css` and edit the four lines under “CHANGE THESE FIRST” (`--paper`, `--brown`, `--blue`, `--orange`).

---

## How to add an artwork

1. Put a photo in `images/art/` (for example `piece-1.jpg`).
2. Open `art.html`.
3. Copy one whole `<figure class="artwork"> ... </figure>` block.
4. Delete the dashed “Photo goes here” box.
5. Remove the `<!--` and `-->` around the `<img ...>` line and point it at your file name.
6. Change the title and caption.

---

## How to add a project

Open `projects.html`. Copy one whole `<article class="project"> ... </article>` block. Change the title, year, and sentences.

---

## How to add a resume PDF

Save your CV as `files/resume.pdf`. The “Download PDF” link on the resume page will then work. You can also type your resume into the labeled sections on that same page.

---

## How to add a paper

Open `publications.html`. Copy one `<li> ... </li>` block inside the numbered list. Replace the example authors, title, journal, and year. Google Scholar is already linked and does not need to be pasted again.

Scholar: https://scholar.google.com/citations?user=FqHgsAQAAAAJ&hl=en

LinkedIn: https://www.linkedin.com/in/michalmerav/

---

## How to publish with GitHub Desktop (first time)

GitHub Desktop is an app that copies this folder to GitHub. GitHub Pages is the free hosting. Together they put your files on the internet.

1. Open **GitHub Desktop**.
2. **File → Add local repository** (or **Create a new repository** if it asks).
3. Choose this folder: `C:\website_test1`.
4. If it says the folder is not a repository yet, click **create a repository**. Use a short description like “personal website”.
5. Click **Publish repository** (or **Publish**).
6. Name it exactly: `michellemerav.github.io`
7. Leave **Keep this code private** **unchecked**. The site needs to be public to be free.
8. Publish.

Wait a few minutes, then open https://michellemerav.github.io in a browser. The first load can take a little while.

If your GitHub username is not `michellemerav`, the address will be `https://YOURUSERNAME.github.io` instead, and the repository name must match that username.

---

## How to update the live site later

1. Edit and save files on your computer.
2. Open GitHub Desktop. You should see the changed files listed.
3. Type a short summary at the bottom left, for example: `add art photos`.
4. Click **Commit to main**.
5. Click **Push origin**.

After a minute or two, refresh the live website.

---

## If something looks broken

- **Menu goes to a missing page:** check that you did not rename `index.html`, `art.html`, `projects.html`, `resume.html`, or `publications.html`.
- **Colors did not change:** you edited `style.css` — save it, then hard-refresh (Ctrl+F5).
- **Photo does not show:** the file name in the HTML must match the file name in the folder, including `.jpg` vs `.png`.
- **PDF link does nothing useful:** the file must be named `files/resume.pdf` exactly.
- **Live site is old:** make sure you clicked **Push origin** in GitHub Desktop, then wait a minute.
