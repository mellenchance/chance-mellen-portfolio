# Chance Mellen — Portfolio (v2, improved)

One HTML file, no install, no terminal. Double-click **`index.html`** to open
it in your browser.

## What's different from the first draft you saw

This version keeps the parts worth keeping from the file you uploaded —
the light/dark toggle, the "Stills" photo grid, the lightbox — and fixes
what wasn't working:

- **A real full-screen looping video on the homepage** (this was missing —
  the previous file only had a small video box buried inside the Work page).
- **No invented client names.** The uploaded file had project names that
  read like real companies and people (a healthcare system, a car
  dealership, a tennis legend's name). Those are gone, replaced with
  clearly-marked placeholders you fill in with your real projects.
- **A proper About page**, separate from Contact.
- **A simpler Contact page** — direct email/phone/social links instead of
  a form that didn't actually send anywhere.
- **One editable `CONTENT` object** instead of data scattered through the
  page, so adding a project or changing your bio is a matter of editing a
  few lines instead of hunting through HTML.

## To edit your content

Open `index.html` in a plain text editor (right-click → "Open with" → a text
editor, not a browser). Find:

```
const CONTENT = {
```

Everything you'd want to change is inside: your name, bio, contact info and
socials under `site`, the homepage video under `hero`, your films under
`projects`, and your photos under `stills`.

**To add a project:** copy one whole block from `projects` (from `{` to
`},`), paste it into the list, change `title`, `subtitle`, `thumbnail`, and
`description`. Give it a unique `slug`.

**To add a still/photo:** same idea, inside the `stills` list.

**To remove one:** delete its whole block.

Save the file, refresh the page in your browser.

## Replacing placeholders before launch

- `/videos/hero-desktop.mp4`, `/videos/hero-mobile.mp4`,
  `/images/hero-poster.jpg` — the homepage background film. Currently a
  plain placeholder clip. See the main portfolio README (or ask me) for
  compression tips when you export your own footage.
- `/images/project-placeholder-1.jpg` (2, 3) — swap for real project stills.
- `/images/still-placeholder-1.jpg` through `-6.jpg` — swap for real photos.
- `/images/portrait.jpg` — swap for a real photo of you.
- `CONTENT.site.bio` — the second paragraph is marked `[Replace with ...]`.

## The optional "reel" on the Work page

There's a spot at the top of the Work page for a second, quieter showreel
loop (separate from the homepage hero). It's off by default. To turn it on,
set `CONTENT.reel.video` to a video file path — leave it as `""` to keep it
hidden.

## A note on the dark/light toggle

This is a nice touch kept from your original file — it remembers the
visitor's choice using their browser's local storage. No account, no
tracking, nothing sent anywhere.

## Sharing this online (optional)

This version is built to be opened locally, or the whole folder shared with
someone else to open the same way. If you want a real web address later
(so anyone can visit without you sending them a folder), ask me — hosting it
takes about five minutes and stays free.
