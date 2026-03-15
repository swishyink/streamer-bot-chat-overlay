# Streamer.bot Chat Overlay

A highly customizable, single-file HTML chat overlay designed for [Streamer.bot](https://streamer.bot/). This overlay brings dynamic, stylish, and highly configurable chat visualization to your stream. It supports classic scrolling chat, Niconico-style passing messages, and various customized animations.

## ✨ Features

- **No Server Required:** It's a single `overlay.html` file. Just add it as a Browser Source in OBS.
- **Direct Streamer.bot Integration:** Connects directly via Streamer.bot's WebSocket server to listen to chat messages, cheers, raids, follows, and subscriptions.
- **Live Control Panel:** Open `overlay.html` in a normal web browser to access a comprehensive, live-updating settings panel.
- **Multiple Display Modes:**
  - Classic Vertical or Horizontal scrolling.
  - "NicoNico" mode (messages sliding horizontally across the screen).
- **Extensive Theming & Styles:**
  - Frost glass, neumorphic, neon glow, editorial brutalist, and more bubble styles.
  - Customizable fonts, colors, borders, and text shadows.
  - Per-user color palettes and Twitch-native role colors.
- **Rich Emote Support:** Integrates natively with Twitch emotes and emojis.
- **Animations:** Floating, plastering, swinging, and sliding entry/exit animations for chat bubbles.
- **Import/Export:** Save and manage multiple profiles or share your custom configurations as JSON.

## 🚀 Setup Instructions

### 1. Configure Streamer.bot

Before using the overlay, you need to ensure Streamer.bot's WebSocket server is active:
1. Open **Streamer.bot**.
2. Go to `Servers/Clients` -> `WebSocket Server`.
3. Check **Auto Start** and click **Start Server**.
4. Take note of the Port (default is usually `8080`) and Endpoint (default is `/`).

### 2. Add to OBS (or other streaming software)

1. Add a new **Browser Source** to your scene.
2. Select **Local file** and browse to the `overlay.html` file.
3. Set the width and height (e.g., `1920` x `1080` for full screen, or a specific region if you prefer a floating chat box).
4. Click **OK**. The overlay will automatically attempt to connect to Streamer.bot (usually `ws://127.0.0.1:8080/`).

> **Note:** The settings test panel is deliberately hidden when loaded inside OBS so it doesn't appear on your stream.

### 3. Customize Your Overlay

To customize the look and feel of the overlay:
1. Double-click the `overlay.html` file to open it in your regular web browser (Chrome, Firefox, Safari, etc.).
2. You will see the **Control Panel** on the left side of the screen.
3. Use the dropdowns, sliders, and color pickers to tweak the design in real-time.
4. Click **Spawn Test** or **Send** to preview how messages will look.
5. Once you are happy with the setup, the settings are automatically saved to your browser's local storage. You can also **Save Profile** or **Export** your config from the bottom of the panel.

## ⚙️ Key Functionality & Settings

- **Source Mode:** Choose between 'Streamer.bot' or pure Demo mode.
- **Movement Mode:** Dictates how bubbles enter the screen (Scroll, Float, Plaster, Zoom, Swing).
- **Bubble Effects:** Choose the background wrapper for messages (e.g., Rounded, Frosted Glass, Neumorphic, Cyberpunk).
- **Event Toggles:** You can independently turn on or off stream events like Follows, Subs, Cheers, and Raids from appearing in the chat feed.
- **Custom CSS:** A built-in editor lets you inject custom CSS for complete control over the layout.

## 📝 License

This project is provided as-is. Feel free to modify and customize it for your own stream!

---

> [!NOTE]
> This documentation was written by an AI coding assistant.
> Inspired by and based on the concepts from [showmy.chat](https://github.com/BenDMyers/showmy.chat) by [Ben Myers](https://github.com/BenDMyers).
