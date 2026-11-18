# Flick Posts

Two-phone AR rugby kicking game. One phone is the goal marker, the other tracks it with the camera.

## Deploy on Vercel

1. Put `index.html`, `vercel.json` and this README at the **root** of a GitHub repo (not inside a subfolder, and not as a zip).
2. In Vercel: Add New > Project > import the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Root Directory: `./`.
4. Deploy, then open the `https://` URL on both phones.

Camera and motion access only work over HTTPS. Open the link in Safari (iPhone) or Chrome (Android), not inside another app's built-in browser.
