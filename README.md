# HYROX Dallas Tracker — PWA

Hybrid athlete training command center. Deploy to Vercel, install on your iPhone.

## Deploy in 5 steps

### 1. Create a GitHub account
Go to github.com → Sign up (free). Skip if you have one.

### 2. Create a new repository
- Click the **+** icon (top right) → New repository
- Name it: `hyrox-tracker`
- Set to **Public**
- Click **Create repository**

### 3. Upload these files
On the repository page, click **uploading an existing file** and drag the entire contents of this folder:
```
index.html
manifest.json
sw.js
vercel.json
icons/
  icon-192.png
  icon-512.png
```
Click **Commit changes**.

### 4. Deploy with Vercel
- Go to vercel.com → Sign up with GitHub (free)
- Click **Add New Project**
- Select your `hyrox-tracker` repository
- Click **Deploy** — no settings to change

Vercel gives you a URL like `hyrox-tracker.vercel.app`.

### 5. Install on iPhone
- Open Safari on your iPhone
- Navigate to your Vercel URL
- Tap the **Share** button (box with arrow pointing up)
- Tap **Add to Home Screen**
- Tap **Add**

The app now lives on your home screen like any native app. Works offline.

## Features
- Dashboard with live KPIs and HR zone display
- Session logging with Apple Watch metrics (HR zones, calories, distance)
- Exercise logging with sets/reps/weight
- RPE slider + reflection notes
- Full session history
- Phase 1 program reference (all 6 days, expandable)
- 6-week stability/mobility progress tracker
- Time trial benchmark tracker with delta vs. target

## Data
All data stored locally in your browser's localStorage. It persists between sessions and survives app restarts. If you want cloud backup in the future, that requires a backend (Supabase, Firebase, etc.) — easy to add later.
