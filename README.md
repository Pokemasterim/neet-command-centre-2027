# NEET Command Centre 2027 — v2.2 (Auto-Build & Auto-Release APK)

This repository automatically compiles **NEET Command Centre 2027 (v2.2)** into an Android APK with native locked-screen alarms (`@capacitor/local-notifications`) and publishes it straight to **GitHub Releases**.

## One-Time Setup (4 Steps)

1. **Create a Public GitHub repository** (e.g. `neet-command-centre-2027`).
2. **Upload these files** to the root of your repository:
   - `package.json`
   - `capacitor.config.json`
   - `www/index.html`
   - `.github/workflows/build-apk.yml` *(create via **Add file → Create new file** if your browser skips hidden `.github` folders)*
3. **Wait ~3–4 minutes** in the **Actions** tab. When finished, your APK is automatically published under **Releases** as `NEET-Command-Centre-2027.apk`.
4. **Link your Netlify Download Page** to your permanent always-latest APK link:
   ```
   https://github.com/YOUR_USERNAME/YOUR_REPO/releases/latest/download/NEET-Command-Centre-2027.apk
   ```

## Releasing Future Updates
1. Replace `www/index.html` in GitHub (or run **Actions → Build & Release NEET Command Centre APK → Run workflow** with a new tag like `v2.3`).
2. Drag the same updated `index.html` to `neetcommandcentre.netlify.app` for iOS/PC web users.
3. Your Netlify download page automatically points to the newest APK — no link edits required!
