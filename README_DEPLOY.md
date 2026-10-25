# ChatSweep Privacy Policy — RevCore Astra

This folder contains a standalone, responsive privacy-policy site for the ChatSweep Chrome extension, version 0.10.5. No JavaScript, tracking pixels, analytics or external fonts are used by this static site.

## Files
- `index.html`: public Privacy Policy landing page
- `privacy.html`: same policy at a distinct path
- `styles.css`: responsive light/dark styling
- `favicon.png`: ChatSweep logo bundled with the user-provided extension

## Publishing on Render (same host as the MediaDock policy approach)
1. Review and approve the actual policy text, especially the publisher identity, support contact, data handling and retention descriptions.
2. Create a NEW GitHub repository for the ChatSweep privacy page, separate from the extension source, and upload these four site files to its root. Do not upload the whole extension ZIP here.
3. In Render, select **New > Static Site**, connect that repository, and choose its branch.
4. Build command: `echo 'No build step required'`
5. Publish directory: `.` (the repository root)
6. Deploy. Render will issue a unique **onrender.com** HTTPS URL. Open it and verify that it publicly shows the ChatSweep Privacy Policy without a login or 404.
7. Enter the **actual verified live HTTPS URL** into ChatSweep's Chrome Web Store **Privacy policy URL** field.

Do NOT use `https://chatsweep-privacy-policy.onrender.com/` unless you have actually deployed the website and verified that this URL is assigned to you.

## Release blockers to revisit
- The uploaded ChatSweep v0.10.5 extension ZIP still contains `legal/privacy.html` and `legal/terms.html` pages marked **DRAFT** and containing publisher/legal placeholders. A future corrected extension upload is needed before submission; this separate public website alone does not fix bundled drafts.
- RevCore Astra is the display/publisher name shown in Chrome Web Store. Confirm whether this is also the legally appropriate operator name for your publishing jurisdiction; add any legally required entity/address/dispute information after review.
- Verify Chrome Web Store data-use declarations and any need for prominent in-product disclosures/consent. The policy is based on source inspection of ChatSweep v0.10.5, not independent network traffic testing across all provider websites.
- Confirm your support inbox is monitored.
- This is a prepared policy for owner review; not a guarantee of legal compliance in every jurisdiction.

Reference: https://developer.chrome.com/docs/webstore/program-policies/privacy
