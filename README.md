# Morsegram — Exteragram Plugin

An [Exteragram](https://exteragram.app/) plugin that automatically converts your outgoing messages to Morse code, with a built-in decoder accessible from the message context menu.

## Features

- 🔡 **Auto-encode** — every message you send is automatically converted to Morse code before delivery
- 🔍 **Decode on demand** — long-tap any message and choose **"Decode Morse"** to see the decoded text in a dialog
- 🌍 **Multilingual support** — handles Latin letters, Cyrillic letters, digits, and common punctuation
- ⚙️ **Toggle switch** — enable or disable encoding from the plugin settings without uninstalling

## Requirements

| | |
|---|---|
| Exteragram | ≥ 11.12.0 |

## Installation

1. Open **Exteragram → Settings → Exteragram → Plugins**
2. Tap the **+** button and choose `morse_code.plugin`
3. Enable the plugin — that's it!

## Usage

### Sending a Morse-coded message
Just type your message and hit **Send** as usual. The plugin intercepts the message and converts it to Morse code automatically (when encoding is enabled in settings).

### Decoding a received message
1. Long-tap the Morse-coded message
2. Select **"Decode Morse"** from the context menu
3. A dialog will show the original Morse and the decoded text

### Settings
| Option | Description | Default |
|---|---|---|
| Encode outgoing messages | Automatically converts your messages to Morse code before sending | ✅ Enabled |

## Morse code table

The plugin encodes/decodes **Latin** (A–Z), **Cyrillic** (А–Я), **digits** (0–9), and a wide range of punctuation and special characters:

```
. , ; : / ( ) ! ? _ " ' & - + = @ $
```

## Author

**@fiudeus**

## License

This plugin is provided as-is. Use at your own risk.
