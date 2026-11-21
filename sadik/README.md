# Sadik 🌲🚗 (صديق = friend)

Find classmates going your way to USJ: same area + same time = one car instead of many.

- **Phone view:** `index.html`. Classmates scan the QR code, enter first name, area, time, and car.
- **Big screen view:** `index.html?screen`. Shows the QR code, a live counter, and the ride groups.

Without Firebase, the app runs in **demo mode** (syncs only between tabs on one computer). To make 16 phones sync live, follow the 2 steps below (~10 minutes).

---

## Step 1: Firebase (free, live database)

1. Go to https://console.firebase.google.com → **Add project** → name it `sadik` → you can turn off Google Analytics.
2. Left menu → **Build → Realtime Database** → **Create database** → pick a location (e.g. Belgium / europe-west1) → choose **Start in test mode**.
3. Go to ⚙️ **Project settings** → scroll to **Your apps** → click the **`</>` (Web)** icon → name it `sadik` → **Register app**.
4. Copy the `firebaseConfig = { ... }` block it shows, and paste it over the one at the top of the `<script>` in `index.html`.
   - Make sure it has a `databaseURL` line. If not, copy the URL from the Realtime Database page (it looks like `https://sadik-xxxx-default-rtdb.europe-west1.firebasedatabase.app`).

> Test mode lets anyone read and write for 30 days. That's fine for a class demo, but don't put real personal data in it.

## Step 2: Put it online with GitHub Pages (free)

1. On GitHub (Edwinuniv) → **New repository** → name it `sadik` → Public → Create.
2. **Add file → Upload files** → upload `index.html` (and this README) → Commit.
3. **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save.
4. After about 1 minute your app is live at:
   - Phones: `https://edwinuniv.github.io/sadik/`
   - Big screen: `https://edwinuniv.github.io/sadik/?screen`

## Before the presentation

- Open `?screen` on the class computer and test with 2–3 friends' phones.
- **Reset all** (click twice) clears the test data so the screen starts empty in class.
- **+ Add fake classmate** adds a pretend student, useful if few people scan or the room is slow.
- Backup plan: record your screen during a test, in case the internet fails.
