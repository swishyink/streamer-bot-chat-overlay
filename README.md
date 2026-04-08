# Streamer Tools

A collection of professional, lightweight, browser-based overlays and utilities designed for live streaming. These tools are built as standalone HTML/JS files perfectly optimized for OBS Studio Browser Sources.

## 🛠 Included Tools

### 1. Pattern Studio (`pattern.html`)
A high-performance HTML physics engine that generates dynamic, infinitely moving grid backgrounds and intermission overlays directly inside OBS.
- **Glassmorphism UI:** Complete modern frosted-glass layout for aesthetic configuration.
- **High-Performance Physics:** Uses delta-time frame tracking and dynamic viewport culling to maintain buttery-smooth 60 FPS natively without exhausting browser CPU limits.
- **Rich Asset Control:** Alternating grids, per-asset 90° rotation, adjustable gaps, rotation angles, and scrolling speeds.
- **Production File Exports:** Download fully baked, persistent production HTML files with your exact configurations hard-coded inside. Bypass all JavaScript initialization bottlenecks when booting up scenes in OBS.
- **Import Presets:** Drop any downloaded pattern file back into the Studio to instantly restore your layout and tweak it further.

### 2. Swishy Chat Overlay (`overlay.html`)
A highly customizable, single-file HTML chat overlay designed seamlessly for [Streamer.bot](https://streamer.bot/).
- **Dynamic Connection:** Connects natively via Streamer.bot's WebSocket server to parse live chats, cheers, raids, follows, and subscriptions.
- **Live Control Panel:** Accessible via local browser for complete real-time aesthetic control. Automatically hides configuration panels when loaded natively in OBS.
- **Rich Emotes & Animations:** Integrates Twitch emotes gracefully with plastering, swinging, scrolling, and floating entry sequences. Includes dark/light text themes, threading, and crossed-out moderation filtering.

## 🚀 Setup Instructions

All tools in this repository are designed to run fully locally without dependencies.

### Pattern Studio Setup
1. Open `pattern.html` in your web browser (Chrome, Firefox, Safari).
2. Configure your pattern grid using the left-hand slider panel. Upload custom image URLs or browse local files.
3. Click "Download Production File" at the bottom of the config.
4. Add that newly downloaded `.html` file to OBS as a **Browser Source** (Check "Local file").
5. *(Optional)* Host `pattern.html` natively on a cloud VPS or NGINX web server to access it perpetually via a web URL.

### Chat Overlay Setup
1. Open **Streamer.bot**, navigate to `Servers/Clients` -> `WebSocket Server`, check **Auto Start**, and click **Start Server**.
2. Double click `overlay.html` in your browser to customize your aesthetic and theme via the live control panel. Settings automatically save to local storage.
3. Add `overlay.html` to OBS as a **Browser Source** (Check "Local file", set Width/Height). It will instantly connect to Streamer.bot in the background.

## 📝 License
This project is provided as-is. Feel free to modify, break, or repurpose any codebase for your own stream!

---

> [!NOTE]
> This documentation was written by an AI coding assistant.
> The Chat Overlay was inspired by and based on the concepts from [showmy.chat](https://github.com/BenDMyers/showmy.chat) by [Ben Myers](https://github.com/BenDMyers).
