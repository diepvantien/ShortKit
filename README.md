# 🎬 ShortKit — The Ultimate Chrome Extension for TikTok

[![Chrome Web Store](https://img.shields.io/badge/Chrome_Web_Store-Install-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://chrome.google.com/webstore/detail/YOUR_EXTENSION_ID)
[![Download ZIP](https://img.shields.io/badge/Download-Latest_ZIP-success?style=for-the-badge&logo=github)](https://github.com/diepvantien/Tiktok-Pro-Tools/archive/refs/heads/main.zip)
[![Version](https://img.shields.io/badge/Version-1.1.0-fe2c55?style=for-the-badge)]()

> Transform your TikTok web experience with professional-grade audio, video, and productivity tools — all running locally in your browser with zero tracking.

---

## ⚡ Why ShortKit?

| Problem | Solution |
|---|---|
| Videos stop when you switch tabs | **Background Play** keeps audio going |
| Audio is too quiet on some videos, too loud on others | **Adaptive Volume Normalizer** auto-balances |
| Can't download videos without watermark | **One-click HD download** (MP4 + MP3) |
| Shop videos blocked in your region | **Shop Unlocker** plays them instantly |
| Spending too much time scrolling | **Daily Limit** reminds or blocks you |
| Want to see product details without leaving the feed | **Product Viewer** shows price, rating, seller |

---

## ✨ Full Feature List

### � Advanced Audio
- **8-Band Equalizer** — presets: Bass Boost, Treble, Vocal, Pop, Rock, Electronic, Jazz, Classical, Dance, Movie + custom curve
- **Adaptive Volume Normalizer** — quiet videos get louder, loud ones soften (real-time RMS-based)
- **360° Spatial Audio (8D)** — immersive rotating stereo field
- **Playback Speed** — 0.25× to 4× with one-click presets

### 📺 Video Tools
- **Background Play** — audio keeps playing when tab is hidden
- **Smart Auto-Pause** — pauses TikTok when other tabs play media
- **Rotate Video** — 90°/180°/270° with pure black letterbox
- **Smart Zoom** — cursor-following region zoom, scroll wheel to adjust (1.2×–5×)
- **Clean Mode** — hides text overlays, descriptions, UI clutter (also in fullscreen)

### 📥 Download & Shop
- **Inline Download Button** — appears on every video (hover to reveal)
- **LIVE Download** — record a live broadcast or copy its FLV/HLS stream link, resolved from the channel in the address bar
- **URL Download Box** — paste any TikTok link to get HD MP4 / MP3
- **3-Provider Failover** — tikwm → douyin.wtf → tiklydown (always works)
- **Shop Video Unlocker** — plays region-restricted TikTok Shop videos
- **Product Viewer** — bottom-left pill shows product name; tap for full details (price, ★ rating, reviews, seller, image, shop link)

### ⌨️ Keyboard Shortcuts
Act on the video you're watching (ignored while typing in a search/comment box):
- **← / →** — seek −3s / +3s
- **, / .** — slower / faster playback
- **Z** — toggle Smart Zoom
- **A** — add to Playlist
- **S** — capture the current frame (screenshot)

### 🧹 Account Cleanup
- **Bulk Unfollow** — scan your Following list, select & run
- **Bulk Unlike / Remove Favorites / Undo Reposts** — scan profile tabs
- **Smart Scan** — auto-opens the right tab, auto-scrolls to load items
- **Human-like execution** — randomized delays, DOM-only clicks, no API abuse

### ⏱ Productivity
- **Watch-Time Dashboard** — today's videos + minutes, 7-day bar chart
- **Watch History** — last 200 videos with thumbnails, duration, username (grid view)
- **Daily Limit System** — set max videos/day or minutes/day
  - *Remind mode*: friendly popup with witty messages you can dismiss
  - *Block mode*: overlay locks the page, pauses all videos until you clear the limit

---

## 🚀 Installation

### From Chrome Web Store (Recommended)
1. Visit the [Chrome Web Store page](https://chrome.google.com/webstore/detail/YOUR_EXTENSION_ID)
2. Click **"Add to Chrome"**
3. Go to [tiktok.com](https://www.tiktok.com) and click the extension icon

### Manual Install (Developer Mode)
1. [Download the ZIP](https://github.com/diepvantien/Tiktok-Pro-Tools/archive/refs/heads/main.zip) and extract
2. Open `chrome://extensions/` → enable **Developer mode**
3. Click **"Load unpacked"** → select the extracted folder
4. Open TikTok and enjoy!

---

## 🖼 Screenshots

<!-- Add 3-5 screenshots here showing the popup, product viewer, download menu, EQ, etc. -->

| Popup Controls | Product Viewer | Download Menu |
|---|---|---|
| ![popup](screenshots/popup.png) | ![product](screenshots/product.png) | ![download](screenshots/download.png) |

---

## 🔒 Privacy & Security

- **Zero tracking** — no analytics, no telemetry, no background data collection
- **100% local storage** — settings, history, stats stay in your browser
- **No account access** — never reads your TikTok password, cookies, or DMs
- **Transparent network** — only contacts third-party APIs when YOU click download/shop-unlock, sending only the public video URL
- **Stealth design** — minimal DOM/API intervention to avoid triggering TikTok's security systems

[Read full Privacy Policy →](PRIVACY_POLICY.md)

---

## 📊 How It Compares

| Feature | ShortKit | Other Extensions |
|---|---|---|
| Background Play | ✅ | ✅ (some) |
| 8-Band EQ + Presets | ✅ | ❌ |
| Adaptive Volume Normalizer | ✅ | ❌ |
| 360° Audio | ✅ | ❌ |
| Video Rotate + Zoom | ✅ | ❌ |
| Shop Video Unlocker | ✅ | ❌ |
| Product Viewer (price/rating) | ✅ | ❌ |
| Watch History (thumbnails) | ✅ | ❌ |
| Daily Limit (block mode) | ✅ | ❌ |
| Account Cleanup (bulk) | ✅ | ❌ |
| Multi-provider download | ✅ (3 fallbacks) | ✅ (usually 1) |
| Privacy-first (no tracking) | ✅ | ⚠️ (varies) |

---

## 🛠 Tech Stack

- **Manifest V3** (Chrome's latest extension platform)
- Pure vanilla JavaScript — no frameworks, no build step
- Content script + page-world hook architecture
- Declarative Net Request for header modifications
- Chrome Storage API (sync + local)
- Web Audio API (EQ, compressor, stereo panner, analyser)
- Canvas API (video frame capture, history thumbnails)

---

## 📝 Changelog

### v1.1.0 (Latest)
- ✨ **Anonymous Story View** — watch public Stories without leaving a "seen" on your account
- ✨ **LIVE download** — record a broadcast or copy its FLV/HLS link, resolved from the `@channel` in the address bar
- ✨ **Bulk download** — grab every video on a profile, to a folder or as a `.txt` link list
- ✨ **Shop-video Cinema popup** — plays region-locked shop clips with sound, plus an on-device product QR code
- ✨ **Keyboard shortcuts** — ← / → seek ±3s, `,` / `.` speed, `Z` zoom, `A` playlist, `S` screenshot
- 🔧 Clean Video Mode now also hides overlays in fullscreen
- 🔧 Create a playlist inline from the in-video menu (no more browser prompt)
- 🔧 Most features are **ON by default** now (except Clean Mode)
- 🐛 Fixed duplicate toolbar showing when opening a video on search / profile pages
- 🐛 Fixed frozen-frame (thumbnail + audio only) caused by injecting UI into the player
- ❌ Removed the **Block Keywords** feature
- 🔒 Dropped the `tabs` permission — no more "read browsing history" warning

### v1.0.0
- ✨ Rebranded to **ShortKit**
- ✨ 8-band Equalizer with presets + custom curve
- ✨ Background Play, Smart Auto-Pause, playback speed
- ✨ Adaptive Volume Normalizer, 360° spatial audio
- ✨ Rotate, Smart Zoom, Clean Mode
- ✨ Inline / URL download (MP4 + MP3) with 3-provider failover, subtitle `.srt` download
- ✨ Playlist player (vinyl / sound-wave themes, shuffle, repeat, import/export)
- ✨ Watch-time dashboard, watch history, daily limits
- ✨ Account cleanup (bulk unfollow / unlike / remove favorites / undo reposts)
- ✨ Product Viewer for shop videos

---

## ☕ Support the Developer

If this extension improves your daily TikTok experience, consider supporting continued development:

[![Buy Me A Coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/tixuno)
[![Donate Momo](https://img.shields.io/badge/Donate-Momo-AE2070?style=for-the-badge&logo=appveyor&logoColor=white)](https://me.momo.vn/OeIGiJsViJfDfntmiRId)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/diepvantien)

**Bank Transfer (Vietnam):**
- Bank: Vietinbank (ICB)
- Account: `109866849450`
- Name: `DIEP VAN TIEN`
- Message: `Ung ho Diep Van Tien`

---

## 👨‍💻 Author

**Diep Van Tien** — Full-stack developer & Chrome extension specialist

- 🌐 GitHub: [@diepvantien](https://github.com/diepvantien)
- 📧 Email: dieptien290620@gmail.com

---

## 📜 License

**Custom MIT License**
- ✅ Personal use: Free and unrestricted
- 💼 Commercial use: Requires a paid commercial license — [contact the author](mailto:dieptien290620@gmail.com)

See [LICENSE](LICENSE) for full terms.

---

## 🌟 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=diepvantien/Tiktok-Pro-Tools&type=Date)](https://star-history.com/#diepvantien/Tiktok-Pro-Tools&Date)

---

<p align="center">
  <b>Made with ❤️ for TikTok power users</b><br>
  <sub>If you find this useful, give it a ⭐ on GitHub — it helps others discover it!</sub>
</p>
