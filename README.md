# 🧊 Hoth — frozen meat inventory tracker

A tiny, private app for tracking what's in your freezer and knowing when to reorder.
It's a single file (`index.html`). No accounts, no cloud, no subscription.

**Your data stays on your phone.** Everything you enter is saved only in your
phone's own browser storage — it is never uploaded anywhere.

## What it does

- **Add items** — name, how many you have, and a "reorder at" number.
- **Add/remove stock** — big **+** and **−** buttons; tap as you use things up.
- **Reorder alerts** — when an item drops to its "reorder at" number or below,
  a yellow **"⚠️ Time to reorder"** banner appears at the top listing what's low.
- **Edit or delete** — tap the ✎ pencil on any item.
- **Backup** — tap the **⋯** button (top right) to **Export** your list to a file
  or **Import** it back. Your safety net, since the data lives only on the device.

## How to put it on your iPhone home screen

The app needs to open at a web address (a link) for iOS to let you add it to your
home screen. The **code** at that link contains no personal data — all your
inventory lives only on your phone. You have two ways to get that link:

### Option A — Easiest (recommended): free one-time upload
1. On your Mac, open **https://app.netlify.com/drop** in a browser.
2. Drag the whole **Hoth** folder onto that page.
3. It instantly gives you a link like `https://something.netlify.app`.
4. Open that link **in Safari on your iPhone**.
5. Tap the **Share** button (the square with an arrow) → **Add to Home Screen** → **Add**.
6. Done — a 🧊 Hoth icon is now on your home screen. Tap it and use it like an app.

*(This uploads only the app's code, for free, so your phone has a link to open.
Your freezer data never goes there.)*

### Option B — Fully offline, no upload at all
Open `index.html` directly in a browser on your Mac and use it there. It works
the same, but this way it lives on your computer rather than your phone.

## Good to know

- **Where's my data?** In the browser's local storage on whatever device you
  added it to. If you install via Option A, use the app from the home-screen
  icon each time so your data stays in one place.
- **Backups:** Because it's local-only, the data isn't backed up automatically.
  If you erase Safari's website data or delete the app, the list is gone — so use
  the **⋯ → Export backup file** button now and then to save a copy (it saves to
  your Files / downloads). To restore, tap **⋯ → Import from backup** and pick
  that file. Importing replaces the current list, and it politely ignores any file
  that isn't a Hoth backup.
- **Notifications:** Reorder alerts show inside the app when you open it (a
  yellow banner). A true "buzz me when the app is closed" notification would
  require either a native app or a cloud service — out of scope for this
  local-only version.
