# donburi-labs Nixie Products – Support

Support page for all nixie-style products by **donburi-labs** on Elgato Marketplace.

This repository is for questions, bug reports and feature requests. Product source code is not published here.

## Products

| Product | Platform | Price |
|---|---|---|
| Nixie Clock | CORSAIR iCUE / XENEON EDGE widget | Paid |
| Nixie Time | Stream Deck plugin | Free |
| Nixie Monitor | Stream Deck plugin | Paid |
| Nixie Icon Pack | Stream Deck icons | Free |
| Nixie Icon Pack Animated | Stream Deck icons | Paid |

**Nixie Token Monitor** (Claude Code usage widget) has its own repository. Please report issues there:
https://github.com/donburi-labs-dev/nixie-token-monitor

## How to get help

1. Open a new Issue.
2. Put the product name in the title, e.g. `[Nixie Monitor] Network shows 0`.
3. Include the information listed for your product below.

**Purchases and refunds** are handled by Elgato Marketplace support, not by this repository.

## What to include in a bug report

### Nixie Clock (iCUE)
- Nixie Clock version (shown on the Marketplace page)
- iCUE version
- Widget size (S, M, L or XL)
- A screenshot, if possible

### Nixie Time / Nixie Monitor (Stream Deck plugins)
- Plugin version (shown in Stream Deck)
- Windows version and Stream Deck app version
- What you expected and what happened
- The latest log file from:
  - Nixie Time: `%APPDATA%\Elgato\StreamDeck\Plugins\com.donburilabs.nixietime.sdPlugin\logs\`
  - Nixie Monitor: `%APPDATA%\Elgato\StreamDeck\Plugins\com.donburilabs.nixiemonitor.sdPlugin\logs\`

### Nixie Icon Pack / Nixie Icon Pack Animated
- Pack name and color
- Which icon, and a screenshot of how it looks on your device

## FAQ

### Nixie Monitor

**The CPU value is slightly different from Task Manager.**
Nixie Monitor reads the same counter as Task Manager (% Processor Utility), but the two sample at different moments, and Smoothing (3 s by default) averages the value. Small differences are normal. Set Smoothing to Off to see the instant value.

**Network shows 0 or the wrong adapter.**
The adapter is chosen automatically (connected, has a gateway, fastest link). If you use a VPN or several adapters, select the adapter manually in the Network action settings.

**What is the difference between bps and B/s?**
bps = bits per second (KBPS / MBPS / GBPS), as used by internet providers. B/s = bytes per second (KBYT / MBYT / GBYT), as shown by download managers. 1 B/s = 8 bps.

**What is the anti-poison effect?**
Real nixie clocks cycle through all digits regularly to keep unused cathodes from wearing out. With this option on, the digits cycle 0–9 once a minute. It is purely decorative and off by default.

**Does the plugin send any data?**
No. All values are read locally and are never sent anywhere. To read Windows performance counters, the plugin runs the built-in Windows PowerShell in the background while CPU or Network keys are visible, and stops it when they are removed.

### Nixie Time / Nixie Monitor

**Is macOS supported?**
Not at the moment. Both plugins are Windows only.

## Marketplace links

- Nixie Clock: https://marketplace.elgato.com/product/nixie-clock-bdba2541-a700-46cd-805a-8614429a2dbd
- Nixie Time: https://marketplace.elgato.com/product/nixie-time-a49e70fc-7d09-4a50-bb77-5405e567b381
- Nixie Monitor: (URL will be added after release)
- Nixie Icon Pack: https://marketplace.elgato.com/product/nixie-icon-pack-18727bf7-f8a9-411f-b6bd-54c018d5f4ad
- Nixie Icon Pack Animated: https://marketplace.elgato.com/product/nixie-icon-pack-animated-96c2ee2d-9fa2-44ce-8978-f911e6e3b804

---
© donburi-labs
