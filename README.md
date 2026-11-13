# Stream Setup Map

Draw your streaming or video-meeting setup: computers and their internal cards, capture cards, cameras, mics, mixers, conference gear, software, cables, audio routing and power strip capacity. One page, no install, no account.

## Put it on GitHub Pages

1. Create a repository (public, or private on a paid plan) and upload the three files in this folder: `index.html`, `README.md` and `.gitignore`.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then save.
4. After a minute the app is live at `https://YOUR-USERNAME.github.io/YOUR-REPO/`.

You can also just double-click `index.html` to run it from your own computer.

## Where your data lives

- **Only in your browser.** Every setup is saved in the browser's local storage on the device you are using. GitHub only serves the page; it never receives your setups.
- **Nothing is sent anywhere.** The page has no server, no analytics and no sign-in. It also carries a browser security rule (`connect-src 'none'`) that blocks the page from making network requests with your data.
- **Each person has their own.** Someone else who opens the same link starts with a blank canvas and cannot see yours.
- **One outside request.** The page loads its typeface from Google Fonts. That request carries no setup data. To avoid it, delete the three `<link>` lines for `fonts.googleapis.com` and `fonts.gstatic.com` near the top of `index.html`; the app falls back to your system font.

Because the data is tied to one browser, clearing site data or switching device loses it. Use **Save setup file** to keep a backup (`something.stream-setup.json`) and **Open setup** to load it elsewhere.

## Keeping setups out of the repository

Saved setups describe your own equipment. The included `.gitignore` skips `*.stream-setup.json`, so a setup file dropped into the project folder is not committed by accident. If you upload through the GitHub website instead of git, simply do not upload those files.

## Sharing a setup on purpose

Use **Save image** for a picture, or send someone your `.stream-setup.json` file; they load it with **Open setup**.
