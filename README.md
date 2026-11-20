# Flick Posts

Two-phone AR rugby kicking game. One phone is the goal marker, the other tracks it with the camera.

## Playing

1. **Goal phone:** tap "I'm the goal", lay it flat, screen up, where the posts should stand.
2. **Kicker phone:** tap "I'm kicking" (allow camera and motion access), aim at the goal phone and tap it on screen once to lock its colour.
3. **Goal phone:** tap "Start 20 second timer". The countdown shows on its screen.
4. When it reaches zero the colour disappears and the goal phone returns to the menu. Swap over: the goal phone taps "I'm kicking" and the kicker taps "I'm the goal".

"End timer" on the goal phone stops the countdown early. Scores are kept on each phone until the page is reloaded.

## Deploy on Vercel

1. Put `index.html`, `vercel.json` and this README at the **root** of a GitHub repo (not inside a subfolder, and not as a zip).
2. In Vercel: Add New > Project > import the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Root Directory: `./`.
4. Deploy, then open the `https://` URL on both phones.

Camera and motion access only work over HTTPS. Open the link in Safari (iPhone) or Chrome (Android), not inside another app's built-in browser.
