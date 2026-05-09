# Ramadan's Daily Tracker

A daily habit tracker with pocket money incentives, family dashboard, and Google Drive sync.

---

## FILES IN THIS PACKAGE

```
ramadan-tracker/
├── index.html          ← The entire app (open this)
├── manifest.json       ← Makes it installable on Android
├── sw.js               ← Offline support (service worker)
├── README.md           ← This file
└── icons/
    ├── icon.svg
    ├── icon-192.png
    ├── icon-512.png
    ├── apple-touch-icon.png
    └── favicon-32.png
```

---

## STEP 1 — PUT IT ON GITHUB (free hosting)

1. Go to https://github.com and create a free account
2. Click **New repository**
3. Name it exactly: `ramadan-tracker`
4. Set it to **Public** → click **Create repository**
5. Click **uploading an existing file**
6. Drag and drop ALL files AND the `icons` folder into the upload box
7. Click **Commit changes**
8. Go to **Settings → Pages**
9. Under Source, select **Deploy from branch → main → / (root)**
10. Click **Save**
11. Wait 1–2 minutes, then your app is live at:
    **https://YOURUSERNAME.github.io/ramadan-tracker**

---

## STEP 2 — INSTALL ON MUM'S PHONE (Android)

1. Open **Chrome** on Mum's phone
2. Go to: `https://YOURUSERNAME.github.io/ramadan-tracker`
3. Tap the **three dots menu (⋮)** in the top right
4. Tap **"Add to Home screen"**
5. Name it **Daily Tracker** → tap **Add**
6. It now appears on the home screen like a real app
7. Opens fullscreen — no browser bar, no address bar

---

## STEP 3 — GOOGLE DRIVE SYNC SETUP

### Get your Client ID (do this once):

1. Go to https://console.cloud.google.com
2. Click **Select a project → New Project**
3. Name it `Ramadan Tracker` → click **Create**
4. Go to **APIs & Services → Library**
5. Search **Google Drive API** → click it → click **Enable**
6. Go to **APIs & Services → OAuth consent screen**
   - Choose **External** → click **Create**
   - App name: `Ramadan Tracker`
   - User support email: your email
   - Scroll down → **Save and Continue** through all steps
7. Go to **APIs & Services → Credentials**
8. Click **+ Create Credentials → OAuth 2.0 Client ID**
9. Application type: **Web application**
10. Name: `Tracker Web`
11. Under **Authorised JavaScript origins**, click **+ Add URI**
    - Add: `https://YOURUSERNAME.github.io`
    - Also add: `http://localhost` (for testing)
12. Click **Create**
13. Copy the **Client ID** (looks like: `123456789-abcd.apps.googleusercontent.com`)

### Connect in the app:

1. Open the app and type `alameen2025dashboard` (no box — just type it)
2. The dashboard opens — go to the **Sync & backup** section
3. Paste your Client ID into the input box
4. Tap **Connect** → sign in with your Google account
5. Tap **↑ Sync to Drive** — done, data saved to your Google Drive
6. The Client ID is remembered — you only paste it once

---

## HOW THE APP WORKS

### For Ramadan (daily):
- Opens to Today tab — greets him and shows pocket money
- 6 tasks to complete each day, each one-click and time-stamped
- At **10pm exactly** the day auto-locks — anything not tapped is marked missed
- Can't go back and change a past day
- Subject rotates daily: Physics → Chemistry → Biology → Agric → English → Maths → Further Maths → Civic → Economics

### Pocket money system:
- Starts at ₦200
- Complete **5+ full days** in a week → **+₦100** (max ₦500)
- Less than 5 days → **-₦100** (min ₦0)
- Mum sees the amount on screen every day — she knows what to give

### For you and Fathia (dashboard):
- Type `alameen2025dashboard` anywhere on the app page
- Dashboard appears showing Ramadan's streak, today's progress, money level
- Add other people you're tracking with the + Add button
- Backup and Google Drive sync controls are here too
- Mum and Ramadan never see this — no button, no link

---

## GOOGLE FAMILY LINK (phone bedtime enforcement)

The app logs sleep but can't physically lock the phone — use Family Link for that:

1. Download **Google Family Link** on YOUR phone
2. Download **Google Family Link for children** on Mum's phone
3. Follow the setup to link his Google account
4. Go to his profile → **Daily Activity → Bedtime → set 10:00 PM**
5. His phone locks automatically at 10pm every night
6. You can also block specific apps after set times

---

## DASHBOARD SECRET KEYWORD

`alameen2025dashboard`

Type this anywhere on the app (no text box needed — just type it like a keyboard shortcut).
Works in any browser — Chrome on phone, laptop, anywhere.
