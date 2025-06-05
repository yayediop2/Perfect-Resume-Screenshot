# 📸 Pixel-Perfect 4K Screenshot of an HTML/CSS Resume (When Print to PDF Fails)

I built my resume using **HTML** and **CSS Grid**, and wanted to export it as a clean, professional **PDF**.  
But every tool I tried — browser print, Puppeteer, screenshot extensions — failed to render the layout properly.  
Text was blurry, elements moved, and the design just broke.

---

## ❌ The Problem

I tried everything:

- **Chrome “Print to PDF”** → layout shifted, fonts blurry
- **Online screenshot tools** → compression artifacts, styles lost
- **PDF generators (Puppeteer, extensions)** → CSS Grid & Flexbox were broken
- **OBS / system screenshots** → not sharp enough for zoom or sharing

When you're using **modern layouts (Grid, Flexbox)** with precise spacing and alignment, these methods can easily ruin the visual fidelity of your resume.

---

## ✅ The Solution: Use Chrome DevTools for 4K Screenshots

The solution I found?  
Take a **high-resolution screenshot directly from Chrome DevTools** using a custom device with a high **device pixel ratio** (DPR).  
This approach preserves every detail exactly as rendered in your browser.

---

### 💡 Why This Works

- Renders your resume like a real browser (no print stylesheet weirdness)
- Keeps **crisp fonts** and accurate **CSS Grid/Flexbox** layout
- Fully customizable resolution and scaling
- Outputs a lossless **PNG image** — perfect for conversion or printing

---

## 🛠️ Step-by-Step Guide

1. Open your resume in **Google Chrome**(or **Chromium**)
2. Press `Ctrl + Shift + I` (or `Cmd + Option + I` on Mac) to open **DevTools**
3. Press `Ctrl + Shift + M` to toggle **Responsive Design Mode**
4. Click the device dropdown > **Edit...** > **Add custom device**
   - Name: `4K Screenshot`
   - Width: `900`
   - Height: `1520`
   - Device Pixel Ratio: `4`
   - Type: `Desktop`
   - Leave User Agent blank
   - Click **"Add"**
5. Select `4K Screenshot` from the dropdown
6. Set zoom to **75%** (or tweak as needed to fit content)
7. (Optional) Reload the page to ensure everything renders properly
8. Click the three-dot menu in DevTools > **Capture screenshot** or **Capture full-size screenshot**

---

## 📄 From Screenshot to PDF

You’ll now have a **crystal-clear PNG** image of your resume.

To convert it to PDF:

- Use [png2pdf.com](https://png2pdf.com) — drag and drop your PNG file(s)
- Combine multiple screenshots into one PDF if your resume spans multiple pages

Now your PDF will look **exactly** like your HTML/CSS version — layout intact, no distortion.

---

## ✨ Bonus Tips

- You can reuse this trick for portfolios, dashboards, or web designs — any layout that breaks when printed.
- For multi-page CVs: take one screenshot per “page height” and merge them later.

---

## 🙌 Reuse & Share

Feel free to fork this repo or reuse the technique in your own workflow!  
If this helped you, share it — it might save someone else hours of frustration 😊
