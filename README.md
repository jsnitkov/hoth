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

## Where it lives

The app is served by GitHub Pages from this repo's `master` branch:
**https://jsnitkov.github.io/hoth/**. Pushing to `master` redeploys it.

The repo is public, but it holds only the app's code. Your freezer list is
never in the repo or on GitHub; it lives only in your phone's browser storage.

The version label at the bottom of the **⋯** menu (commit and build date) is
filled in by GitHub Pages when it deploys, so it is never typed by hand. A copy
opened straight from disk says "local copy" instead.

## How to put it on your iPhone home screen

1. Open **https://jsnitkov.github.io/hoth/** in **Safari** on your iPhone.
2. Tap **Share** (the square with an arrow) → **Add to Home Screen** → **Add**.
3. A 🧊 Hoth icon is now on your home screen. Tap it and use it like an app.

You can also open `index.html` directly in a browser on your Mac. It works the
same, but that copy keeps its own separate list.

## Good to know

- **Where's my data?** In the browser's local storage on whatever device you
  added it to, tied to the site it was opened from (`jsnitkov.github.io`). Use the app
  from the home-screen icon each time so your data stays in one place. If it
  ever moves to a different site (a custom domain or another host), the app
  opens empty there. **Export a backup first**, then import it there.
- **Backups:** Because it's local-only, the data isn't backed up automatically.
  If you erase Safari's website data or delete the app, the list is gone — so use
  the **⋯ → Export backup file** button now and then to save a copy (it saves to
  your Files / downloads). To restore, tap **⋯ → Import from backup** and pick
  that file. Importing replaces the current list after asking. It refuses any file
  that isn't a Hoth backup, and any backup with no items in it.
- **Notifications:** Reorder alerts show inside the app when you open it (a
  yellow banner). A true "buzz me when the app is closed" notification would
  require either a native app or a cloud service — out of scope for this
  local-only version.
