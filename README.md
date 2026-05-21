# Apple Emoji + SF Thonburi for Vesktop / Discord

Make Vesktop/Discord use:

* 🍎 Apple Color Emoji
* 📝 SF Thonburi font

Works on:

* Linux
* Windows
* macOS (Why do u need this lol)
* Flatpak
* Vesktop
* BetterDiscord
* Vencord

This bypasses Electron/Chromium font issues by loading fonts directly through CSS.

---

# Preview

* Apple emojis instead of Noto/Twemoji
* SF Thonburi UI font
* Cleaner Apple-style appearance

---

# Installation

Open:

Settings → Themes → Quick CSS

Paste this CSS:

```css id="f54fny"
@font-face {
  font-family: "Apple Color Emoji";
  src: url("https://github.com/samuelngs/apple-emoji-ttf/releases/download/macos-26-20260219-2aa12422/AppleColorEmoji-Linux.ttf") format("truetype");
}

@font-face {
  font-family: "SF Thonburi";
  src: url("https://github.com/jaruwitaa/Apple-Thonburi-ThaiEng-Font/releases/download/67/SFThonburi-Regular.ttf") format("truetype");
  font-weight: 400;
}

@font-face {
  font-family: "SF Thonburi";
  src: url("https://github.com/jaruwitaa/Apple-Thonburi-ThaiEng-Font/releases/download/67/SFThonburi-Semibold.ttf") format("truetype");
  font-weight: 600;
}

@font-face {
  font-family: "SF Thonburi";
  src: url("https://github.com/jaruwitaa/Apple-Thonburi-ThaiEng-Font/releases/download/67/SFThonburi-Bold.ttf") format("truetype");
  font-weight: 700;
}

:root {
  --font-primary: "SF Thonburi", "Apple Color Emoji", sans-serif !important;
}

body,
.markup_f8f345,
.contents_c19a55,
.messageContent_f9f2ca,
.text-sm-normal__95a78,
.text-md-normal__95a78 {
  font-family:
    "SF Thonburi",
    "Apple Color Emoji",
    sans-serif !important;
}
```

Restart Vesktop/Discord completely after applying.

---

# Notes

* Works even when Discord ignores system emoji fonts.
* Bypasses Electron/Chromium font rendering issues.
* Fonts are loaded directly from GitHub URLs.
* No need to install fonts system-wide.

---

# Credits

Apple Emoji font:
https://github.com/samuelngs/apple-emoji-ttf

SF Thonburi:
https://github.com/jaruwitaa/Apple-Thonburi-ThaiEng-Font
