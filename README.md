# Flick Posts

Two-phone AR rugby kicking game. One phone is the goal marker, the other tracks it with the camera. Every turn lasts 20 seconds, then the phones swap roles.

## How a turn works

1. **Goal phone:** tap "I'm the goal", lay it flat, screen up, where the posts should stand. The first tap asks for camera and motion access on both phones. Allow both: the swap happens later without a tap, so it needs the permissions already granted.
2. **Kicker phone:** tap "I'm kicking", aim at the goal phone and tap it on screen once to lock its colour.
3. **Goal phone:** tap "Start 20 second turn". It counts down 3 seconds, flashes **cyan** for under a second (the start signal), then shows a 20 second countdown.
4. **Kicker phone:** sees the cyan flash, starts its own matching countdown in the top left, and you flick the ball at the posts.
5. At zero the goal phone flashes **green** (the swap signal). The kicker's camera sees it and the kicker becomes the goal. The goal phone becomes the kicker. The new goal phone gets a 6 second "Get ready" countdown and starts the next turn by itself.

The phones talk only through the camera, so the kicker must be pointing at the goal phone when the flashes happen.

If a swap goes wrong: on the goal phone tap **Swap now**, on the kicker open **Settings** and tap **Become the goal**.

## Deploy on Vercel

1. Put `index.html`, `vercel.json` and this README at the **root** of a GitHub repo (not inside a subfolder, and not as a zip).
2. In Vercel: Add New > Project > import the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Root Directory: `./`.
4. Deploy, then open the `https://` URL on both phones.

Camera and motion access only work over HTTPS. Open the link in Safari (iPhone) or Chrome (Android), not inside another app's built-in browser.
