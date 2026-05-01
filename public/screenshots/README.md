# Screenshots

Drop real Markdown Preview screenshots into this folder. The site references them by filename.

## Expected files

| Filename | Used in | Recommended size | Aspect ratio |
| --- | --- | --- | --- |
| `hero@2x.png` | Hero MacBook frame | 2880×1854 (or 3024×1964) | 16:10.3 (full MBP 14" display, includes menu bar) |
| `outline@2x.png` | "Document outline" feature row | 2000×1600 | ~5:4 (window-only) |
| `quicklook@2x.png` | "Quick Look" feature row | 2000×1600 | ~5:4 (window-only) |
| `rendering@2x.png` | "Native rendering" feature row | 2000×1600 | ~5:4 (window-only) |

Until these files exist, the components fall back to a quiet placeholder so the page still renders.

## How to capture

The cleanest captures match what Apple ships on apple.com:

1. **Hero shot** — open the app fullscreen on a 14" MacBook Pro (or 1440×900 logical / 2880×1800 retina). Capture the entire screen with `Cmd+Shift+3`. Keep the menu bar — the MacBook frame's notch overlaps it the same way it does on real hardware.
2. **Window shots (lower sections)** — capture *just the window* with `Cmd+Shift+4` then `Space` to select the window. macOS adds a soft drop shadow; you can disable it with `defaults write com.apple.screencapture disable-shadow -bool true; killall SystemUIServer` if you want the bare window (the AppWindow component adds its own shadow).

## Format

PNG is fine. WebP is smaller. JPG works but loses sharpness on flat UI areas. The components don't require any specific format — any URL works.

## 2x naming

The `@2x` in the filename is just a convention so you remember these are retina-resolution. The site renders them at half size on a 1440px display, so 2880px-wide images are sharp on retina screens.
