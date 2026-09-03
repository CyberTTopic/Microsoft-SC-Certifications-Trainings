# SC-900 Series — How to publish on Dev.to

Everything is ready to paste. Follow these steps once per post.

## 1. Upload the images first

Dev.to hosts images for you: in the editor, click the image icon (or drag the file into the editor) and it returns a URL like
`https://dev.to/social_previews/...` or `https://media.dev.to/...`.

Upload the images, copy each URL, and replace the placeholders in the Markdown:

| Placeholder | Image file | Used in |
|---|---|---|
| `IMAGE_URL_00` | `images/00-cover.png` | Post 0 (also use as **cover_image** for the whole series) |
| `IMAGE_URL_01` | `images/01-domains.png` | Post 0 |
| `IMAGE_URL_02` | `images/02-zero-trust.png` | Post 1 |
| `IMAGE_URL_03` | `images/03-shared-responsibility.png` | Post 1 |
| `IMAGE_URL_04` | `images/04-authn-authz.png` | Post 1 |
| `IMAGE_URL_05` | `images/05-entra-model.png` | Post 2 |
| `IMAGE_URL_06` | `images/06-conditional-access.png` | Post 2 |
| `IMAGE_URL_10` | `images/10-licensing.png` | Post 2 |
| `IMAGE_URL_07` | `images/07-defender-xdr.png` | Post 3 |
| `IMAGE_URL_08` | `images/08-sentinel-vs-defender-cloud.png` | Post 3 |
| `IMAGE_URL_09` | `images/09-purview-lifecycle.png` | Post 4 |
| `IMAGE_URL_11` | `images/11-lab-setup.png` | Post 0 |

All images are 1600×900 PNG, which is the ratio Dev.to uses for cover images.

## 2. Create the post

1. Dev.to → **Create Post** → switch to the **Markdown editor** (top right, "Edit in markdown" / the settings gear).
2. Paste the whole file, front matter included. Dev.to reads the `---` block.
3. Set `cover_image:` to the URL of the image you want at the top.
4. Keep `series: SC-900 Study Series` identical in all six posts — that's what groups them into a series with automatic navigation.
5. Leave `published: false` until you've previewed it, then flip it to `true` (or use the Publish button).

## 3. Cross-link the posts

The posts contain `[Part 1](#)` style links. Once each post is published, come back and replace `#` with the real URL. Do this in order: publish post 0 last if you want every link live from day one, or publish in order and edit post 0 at the end.

## 4. Suggested publishing rhythm

One post every 2–3 days keeps you in the Dev.to feed longer than dumping all six at once. Order:

1. Post 0 (index + lab)
2. Post 1 (concepts)
3. Post 2 (Entra)
4. Post 3 (security)
5. Post 4 (compliance)
6. Post 5 (mock exam) — this one usually gets the most saves

## 5. Tags

Each post has 4 tags (the Dev.to maximum). Good combinations already set:
`microsoft`, `security`, `azure`, `career`, `identity`, `cloud`, `compliance`, `certification`.

## 6. Before you hit publish

- [ ] Replace every `IMAGE_URL_xx` placeholder
- [ ] Check the "Skills measured as of" date on the official study guide and update the note if Microsoft changed it
- [ ] Add your own screenshots from the labs — they're what makes the series yours
- [ ] Add a line about your background at the end of each post (I left one in post 0)
- [ ] Read the post once on a phone; Dev.to traffic is mostly mobile

## 7. Optional upgrades

- Record a 60-second video walking through the Conditional Access lab and embed it in post 2. Video massively increases time-on-page.
- Turn the glossary in post 5 into a downloadable PDF and ask for an email in exchange, if you want to build a list.
- Publish a Spanish version later. There is very little SC-900 content in Spanish and it would rank quickly.

---

## Accuracy notes

- Exam domains and weights follow the SC-900 study guide (objectives updated 28 July 2026): concepts 10–15%, Entra 25–30%, security solutions 35–40%, compliance solutions 15–20%.
- The Microsoft 365 Developer Program no longer accepts personal accounts and requires a qualifying subscription or partner/support membership — that's why the lab uses an Azure free account plus trials instead.
- Microsoft renames products in this space frequently. Before publishing, do a quick pass over product names (Entra External ID, Defender XDR, Purview) against Microsoft Learn.
