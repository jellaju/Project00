# Carepath

A responsive cancer pain tracking companion, ready for a GitHub repository and GitHub Pages. Built with plain HTML, CSS and JavaScript; no build step, API keys, or dependencies.

## Run
Open index.html in a modern browser, or serve this folder with any static HTTP server. Internet is optional for the app; Google Fonts uses an external request and falls back to system fonts.

## Publish on GitHub Pages
1. Create a repository and upload the contents of this folder to its root (index.html must be at the root).
2. In the repository, open Settings > Pages.
3. Select Deploy from a branch, choose main and / (root), and Save.
4. Open the URL GitHub provides after deployment.

No credentials or patient records are included. Do not upload exported patient diaries to a public repository.

## Features
- Pain intensity, location, quality, duration, episode type and free-text notes.
- Timestamped diary with follow-up scores, deletion, date filtering, CSV export and printing.
- Seven-day averages based only on recorded entries; missing days stay blank.
- Clinician-provided care plan and contact details.
- Optional 60-second pause and patient education link.
- Browser-local persistence and explicit deletion of all app records.
- Responsive layouts, labeled forms and keyboard-accessible dialogs.

## Clinical scope and privacy
This is a prototype tracking tool, not a validated medical device or treatment recommendation system. It does not diagnose breakthrough pain, calculate doses, send alerts to clinicians, or monitor emergencies. Episode labels are user selections. Medication instructions must come from the user's clinician. New-pain or severe-score entries show contact guidance, not clinical triage.

Records are stored in unencrypted localStorage on the current browser profile and origin. Other users of that profile can access them. There is no authentication, cloud sync, backend, automatic backup, or regulatory compliance claim. Clearing site data removes records. CSV exports contain sensitive health information. Clinical deployment requires a separate review of clinical safety, accessibility, security, consent and applicable privacy obligations.

The supplied Explorer screenshot shows two PDF filenames, but the PDFs themselves were not supplied or used. This app does not claim to implement or validate those research documents.

## Education source
National Cancer Institute, Pain and Cancer Treatment:
https://www.cancer.gov/about-cancer/treatment/side-effects/pain
Reviewed during development on October 21, 2026. Education is summarized; the linked source is not an endorsement of this app.

## Structure
- index.html: app screens and dialogs
- style.css: responsive styles and print layout
- app.js: local state, diary, exports and interactions

## Verification
JavaScript syntax checked with node --check. No clinical validation has been performed.
