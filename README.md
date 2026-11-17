# LiquidGlassRush

A custom Windows 11 taskbar theme based on **LiquidGlass (Legacy - Alternate)** for the [Windows 11 Taskbar Styler](https://github.com) mod in Windhawk.

This theme retains the translucent frosted-glass aesthetic (`WindhawkBlur`) while fixing visibility issues and reorganizing the layout for cleaner, faster navigation.

## ✨ Key Features & Fixes

* **Three-Zone Split Layout:**
  * **Left:** **Start** and **Search** buttons are anchored to the left edge (`12px` padding).
  * **Center:** Pinned and running app icons stay strictly centered on the taskbar.
  * **Right:** System tray, clock, network, and volume indicators remain aligned to the right.
* **Clear Running vs. Pinned State Indicators:**
  * Unlaunched (pinned-only) apps are dimmed (`Opacity: 0.5`) with no indicator pill.
  * Running apps display a compact indicator pill (`8px`).
  * The active (focused) window is highlighted with an elongated accent-colored pill (`22px`).
  * Apps requiring attention flash with a distinct orange indicator (`#FFFF8C00`).
* **Fixed System Tray Chevron:** Replaces the broken "QR-code-like" glyph with the standard upward arrow (`\uE70E` from `Segoe Fluent Icons`).
* **Unified Glass Aesthetic:** Extends the translucent glass styling and rounded borders to tooltips, `Alt+Tab` switcher, Virtual Desktop bar, Snap Layouts, and overflow flyouts.

## ⚙️ Windows Prerequisites (Required)

Before applying the configuration, adjust your Windows 11 taskbar settings (**Settings → Personalization → Taskbar**) to prevent overlapping elements:

1. **Search:** Set to **Search icon only**.
2. **Taskbar items:** Turn **Off** *Task view*, *Widgets*, and *Copilot*.
3. **Taskbar behaviors → Taskbar alignment:** Set to **Center**.

## 🚀 Installation

1. Install [Windhawk](https://windhawk.net) if you haven't already.
2. Install the **Windows 11 Taskbar Styler** mod by *m417z*.
3. Open the mod's **Settings** and switch to **Textual mode** (under the *Advanced* tab or settings toggle).
4. Copy the `LiquidGlassRush` YAML configuration and paste it into the settings editor.
5. Click **Save settings**.

## 🎨 Customization

You can easily fine-tune spacing and opacity in the `styleConstants` section:

* `LeftPad=12` — Distance of the Start and Search buttons from the left screen edge.
* `LeftGap=2` — Spacing between the Start and Search buttons.
* `DimOpacity=0.5` — Opacity level for pinned (non-running) app icons (`0.0` to `1.0`).
* `CornerRadius=12` / `ElementCornerRadius=8` — Corner radius for the main taskbar/popups and individual buttons.

## 📄 Credits & License

* Built for **Windows 11 Taskbar Styler** by [m417z](https://github.com) (GNU GPL v3.0).
* Based on the **LiquidGlass (Legacy)** theme from the official [Windows 11 Taskbar Styling Guide](https://github.com).
