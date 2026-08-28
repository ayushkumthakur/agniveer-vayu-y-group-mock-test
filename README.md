# AGNIVEER VAYU MATHEMATICS LIVE MOCK TEST

Real public CBT practice architecture using Firebase Authentication, Cloud Functions and Firestore.

## What is included
- 50 Mathematics MCQs, 45-minute server-timed session
- +1 / -0.25 / 0 scoring
- CBT navigation, palette, marked-for-review and clear response
- Secure server-side scoring; answer keys are not public
- Firestore results and public leaderboard
- Protected admin area for results and question management

## Deploy
1. Create a Firebase project.
2. Enable Authentication: Anonymous and Email/Password.
3. Create Firestore.
4. Install Firebase CLI: `npm i -g firebase-tools`, then `firebase login`.
5. Copy `public/firebase-config.js.example` to `public/firebase-config.js` and fill the Firebase Web App config.
6. Create an admin user in Firebase Authentication.
7. Download a Firebase service-account JSON as `serviceAccountKey.json` locally only.
8. Run `node set-admin.js admin@example.com`.
9. Run `node seed.js` to create the initial 50-question Mathematics test and protected answer keys.
10. Run `firebase deploy --only hosting,functions,firestore`.

Public URL: `https://YOUR_PROJECT_ID.web.app/`
Admin URL: `https://YOUR_PROJECT_ID.web.app/admin.html`

Never commit `serviceAccountKey.json` or real credentials.
