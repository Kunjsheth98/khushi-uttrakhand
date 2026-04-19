# 🏔️ Mittal Parivaar — Uttarakhand Yatra 2026

A beautiful, collaborative trip planner for the Mittal family's Kedarnath & Char Dham Yatra.

---

## 🚀 Setting Up the Website (Step by Step)

### Step 1: Enable GitHub Pages

1. Go to your GitHub repository
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Select branch: `main` → Folder: `/ (root)` → Click **Save**
5. Wait 2–3 minutes → your site will be live at `https://yourusername.github.io/your-repo-name`

---

### Step 2: Set Up Firebase (for shared real-time sync)

This is what lets Khushi, Didi, and Kunj all see each other's list items live!

**2a. Create Firebase Project**
1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Click **"Add project"** → Name it `mittal-yatra-2026` → Continue → Disable Google Analytics (optional) → **Create project**

**2b. Create Firestore Database**
1. Inside your project, click **Firestore Database** in the left menu
2. Click **"Create database"**
3. Select **"Start in test mode"** → Next
4. Choose region: `asia-south1 (Mumbai)` → **Enable**

**2c. Get Your Web Config**
1. Click the **⚙️ (Settings)** icon → **Project settings**
2. Scroll to **"Your apps"** → Click the `</>` (web) icon
3. Type any app nickname (e.g. `mittal-web`) → Click **Register app**
4. You'll see a `firebaseConfig` object like this:
```js
const firebaseConfig = {
  apiKey: "AIzaSy...",
  authDomain: "mittal-yatra-2026.firebaseapp.com",
  projectId: "mittal-yatra-2026",
  storageBucket: "mittal-yatra-2026.appspot.com",
  messagingSenderId: "123456789",
  appId: "1:123456789:web:abcdef"
};
```
5. **Copy this entire object**

**2d. Paste Config into index.html**
1. Open `index.html` in any text editor (Notepad works)
2. Find this section near the bottom:
```js
const firebaseConfig = {
  apiKey:            "YOUR_API_KEY",
  authDomain:        "YOUR_AUTH_DOMAIN",
  ...
```
3. Replace `YOUR_API_KEY`, `YOUR_AUTH_DOMAIN`, etc. with your actual values
4. Save the file

**2e. Push to GitHub**
```
git add .
git commit -m "Add Firebase config"
git push
```

Done! 🎉 Share the GitHub Pages URL with Khushi and Didi. All three of you will see each other's items in real time!

---

## 📱 Features

| Feature | Description |
|---|---|
| 🧳 **7 List Categories** | Packing, To-Do, Shopping, Places, Food, Medicines, Documents |
| 👥 **Multi-user Names** | See who added each item (Kunj, Khushi, Didi, etc.) |
| ✅ **Check off items** | Mark things as done — progress bar updates live |
| 🔴 **Delete items** | Tap the trash icon, confirm to remove |
| 🔍 **Filter by person** | See only Khushi's items, or Kunj's, etc. |
| ⏱️ **Live Countdown** | Counting down to May 8, 2026 |
| 🗺️ **Itinerary tab** | Char Dham route preview (full itinerary added later) |
| 📝 **Shared Notes** | One shared notes area for the whole family |
| 📲 **Mobile-first** | Designed for phones — works like an app |

---

## 📂 Files

```
index.html     — The entire website (single file, works offline too!)
README.md      — This setup guide
```

---

## 🕉️ Har Har Mahadev 🏔️
