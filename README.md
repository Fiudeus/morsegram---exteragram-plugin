# Morsegram

Plugin for the Cutegram/CuteMessages plugin framework.

Encodes outgoing messages into:
- **Morse code**
- **NATO phonetic alphabet** (“Альфа Браво Чарли Дельта …”)

Also adds a **Decode** button to the message context menu (long tap).

## Features

- ✅ Encode outgoing messages automatically
- ✅ Multiple modes:
  - **Always encode** (default)
  - **Prefix-only**: encode only when you add a prefix
- ✅ Quick overrides via prefixes:
  - `!m ` — force **Morse**
  - `!n ` — force **NATO**
  - `!raw ` — send without encoding (removes prefix)
- ✅ Decode any received encoded message:
  - Long tap → **Decode**
  - Auto-detects Morse vs NATO
- ✅ Adds **Morsegram Settings** to the **left drawer menu** (if supported by your API build)

## Installation

1. Put `morsegram.py` into your plugins folder.
2. Reload plugins / restart the client.
3. Open plugin settings and configure mode.

## Usage

### Always encode (default)
Any outgoing message is encoded using the **default codec** (Morse or NATO).

### Prefix-only mode
Enable “Prefix-only mode” in settings.

Now encoding happens only if you start the message with:
- `!m ` Example: `!m Hello world`
- `!n ` Example: `!n Hello world`
- `!raw ` Example: `!raw Hello world`

### Decode
Long tap any message → **Decode**.

The plugin will detect:
- Morse: contains only `. - space |`
- NATO: many tokens like `АЛЬФА`, `BRAVO`, `CHARLIE`, etc.

## Notes

- NATO encoding uses Russian names (АЛЬФА/БРАВО/…) by default.
- Decoding understands both RU and EN tokens (e.g. ALPHA/BRAVO or АЛЬФА/БРАВО).
