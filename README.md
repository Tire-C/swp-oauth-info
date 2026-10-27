# SWP — OAuth information

Public, static, informational pages for the **Samsung Workstation Portable** personal Google Drive OAuth client.

This repository deliberately contains **no SWP source code, credentials, tokens, backups, personal files, or private configuration**.

## Pages
- `index.html` — application home page
- `privacy.html` — privacy policy
- `terms.html` — terms of use
- `style.css` — local styling; no JavaScript, trackers or external assets

## Hosting
Publish this repository using GitHub Pages, with **Deploy from a branch → main → /(root)**. The expected address (only once Pages is activated) is `https://tire-c.github.io/swp-oauth-info/`.

Use the publicly accessible home page and privacy policy URLs in Google Cloud Console → Samsung Workstation Portable → Google Auth Platform → Branding. Google may require authorized-domain/ownership verification. Do not mark the OAuth app as published until the console confirms it.

## Security and factual scope
The SWP OAuth client asks for the broad Google Drive `drive` scope, but its own integration is configured to operate within the dedicated SWP folder. The full OAuth grant is broader than that application-side restriction. Backups of SWP checkpoints are encrypted before uploading, while other SWP documents synced to Drive are not necessarily encrypted. OAuth credentials are stored in the rclone configuration on the BitLocker-protected removable Samsung volume. The public website itself neither authenticates users nor accesses Google Drive data.

For anything containing secrets, use private, secure channels — **never public GitHub Issues**.
