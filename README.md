# Wedding Photo Upload Site

Static site, no backend needed. Guests scan a QR code, tap a button, photo goes straight into your Cloudinary media library.

## 1. Cloudinary setup (free, ~2 minutes)
1. Create a free account at cloudinary.com.
2. Go to **Settings → Upload → Upload presets → Add upload preset**.
3. Set **Signing Mode** to **Unsigned**. Save, and note the preset name.
4. On your Cloudinary dashboard, note your **Cloud name**.

## 2. Edit config.json
Fill in:
- `cloudName` — your Cloudinary cloud name
- `uploadPreset` — the unsigned preset name from step 1
- `coupleNames`, `eventDate`, `eventTitle` — shown on the page

## 3. Deploy to GitHub Pages
1. Create a new GitHub repo, upload `index-1.html`, `config.json` (and this README).
2. Repo **Settings → Pages → Deploy from branch → main → / (root)**.
3. Your site will be live at `https://<username>.github.io/<repo>/`.

## 4. Get the QR code
Open the live site, tap **"Show QR code for printing / display"** at the bottom — it generates a QR code of that exact live URL. Screenshot or print it for the venue.

## Viewing uploaded photos
Photos land in your Cloudinary Media Library, inside the folder set in `config.json` (default `wedding-photos`). You can browse, download, or bulk-export them all from there anytime.
