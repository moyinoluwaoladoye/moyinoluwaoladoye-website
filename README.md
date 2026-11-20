# moyinoluwaoladoye.com

Personal academic website for Dr. Moyinoluwa Oladoye.
Plain HTML and CSS — no build step, no framework, nothing to install.

Hosted on Cloudflare Workers. Every change pushed to `main` goes live
automatically within about a minute.

## Where things are

```
wrangler.jsonc        Cloudflare settings. Leave this alone.
public/               The website itself.
  index.html          Home page
  experience.html     Experience + full bio
  publications.html   Publications
  grants.html         Grants and funding
  awards.html         Awards and honours
  media.html          Press and talks
  style.css           All colours, fonts and layout
  img/                Photos
```

## Editing text

1. Open the file here on GitHub, e.g. `public/index.html`
2. Click the **pencil** icon, top right
3. Find the words you want to change. Use **Ctrl+F**.
4. Change the text **between** the tags, not the tags themselves:

   ```html
   <p>Change these words.</p>
   ```

5. Scroll down, click **Commit changes**

Live in about a minute. Refresh the site to see it.

## Changing a photo

Give the new photo the **same filename** as the old one, then:

1. Go to `public/img/`
2. **Add file → Upload files**
3. Drop the new photo in — it replaces the old one
4. **Commit changes**

No code to edit. Filenames in use:

```
headshot.jpg          experience-1.jpg    experience-2.jpg
publications-1.jpg    publications-2.jpg
awards-1.jpg          awards-2.jpg
```

Resize photos to about 1500px wide before uploading. Straight off a
phone they are 5–10 MB each and will make the site slow.

## Changing colours

Everything comes from the top of `public/style.css`:

```css
:root{
  --bg:#f4f6f4;        /* page background */
  --surface:#ffffff;   /* white bands and cards */
  --ink:#10211c;       /* body text */
  --accent:#156b56;    /* green on links and buttons */
  --warm:#a8661a;      /* gold on years and awards */
}
```

Change one value and it updates across all six pages.

Dark mode has its own copies of these further down the same file —
change both if you want dark mode to match.

## If you break something

Click **Commits** at the top of the file list, find the last good one,
and revert it. Nothing is ever lost.
