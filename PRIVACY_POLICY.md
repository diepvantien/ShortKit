# Privacy Policy for ShortKit

**Effective Date:** April 18, 2026

## Introduction
ShortKit ("we", "our", or "us") respects your privacy. This Privacy Policy explains how our Browser Extension collects, uses, and protects your information.

## Data Collection and Usage
ShortKit is designed to function entirely within your local browser. It does not collect, record, or transmit any personally identifiable information, browsing history, or user behavior to external servers, with the following single exception:

**Video/Media Downloading & Playlist Player:** When you explicitly use the "Download" feature, the Playlist player, or the Product/Shop features, the extension sends the relevant TikTok video or product URL to third-party resolver APIs (`tikwm.com`, and as fallbacks `api.douyin.wtf` and `api.tiklydown.eu.org`) solely to retrieve public media links, thumbnails, or basic metadata. No user data, cookies, or account information is sent during this process (requests are made without credentials).

## Permissions Requested and Justifications

To provide its functionality, the extension requires specific Chrome browser permissions:

- **Host Permissions (`*://*.tiktok.com/*`)**: Required to inject scripts that control the video player (e.g., speed control, equalizer, auto-pause) and customize the TikTok interface (e.g., clean mode, removing text overlays). Also used, only when you click download on a live page, to call TikTok's own public live API (`www.tiktok.com`, `webcast.tiktok.com`) to resolve the current broadcast's stream URL.
- **Host Permissions (TikTok CDNs: `*.tiktokcdn.com`, `*.tiktokcdn-us.com`, `*.tiktokcdn-eu.com`, `*.ibytedtos.com`, `*.byteoversea.com`)**: Required to read subtitle tracks, check media file sizes, and save video/live-stream files when you use the subtitle-download, download, and live-download features.
- **Host Permissions (`https://tikwm.com/*`, `https://api.douyin.wtf/*`, `https://api.tiklydown.eu.org/*`)**: Required to resolve watermark-free video/audio download links and playlist media, only when requested by you.
- **Product QR code**: The QR code shown in the shop viewer is generated entirely on your device (bundled generator) and encodes only the plain public product URL. No affiliate code or tracking is added, and no data is sent to any third-party service to create it.

- **`storage`**: Used exclusively to save your local settings, playlists, and usage stats (e.g., playback speed, EQ presets, feature toggles) directly on your device.
- **`downloads`**: Allows the extension to trigger the native Chrome download manager to save videos, audio, subtitles, and screenshots to your device.
- **`declarativeNetRequest`**: Used strictly to modify network locally: (a) to unlock regional shop videos, and (b) when you enable "Anonymous Story View", to remove the Cookie header from TikTok's behavioural report/telemetry requests and to block TikTok's real-time report socket (the channel that reports a Story "seen") so a Story view is not tied to your account. It only targets reporting/telemetry channels — never the feed, video media, or login — works entirely on-device, and sends no data anywhere.
- **`alarms`**: Used to keep the background worker responsive and to perform lightweight background tasks (e.g., daily watch-time limits).

## Analytics and Tracking
We do **not** use Google Analytics, trackers, or any other telemetry to monitor your usage. All "statistics" displayed within the extension (such as videos watched, or watch time) are tracked and stored locally on your device and never leave your browser.

## Third-Party Services
This extension may contact `tikwm.com`, `api.douyin.wtf`, and `api.tiklydown.eu.org` to resolve media download links when you use those features. We are not responsible for the privacy practices of these third-party external services.

## Contact Us
If you have any questions or concerns about this Privacy Policy or your data, please contact the developer at:
**Email:** dieptien290620@gmail.com
