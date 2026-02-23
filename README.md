# Morsegram — Exteragram Plugin

---

## 🇷🇺 Русский

Плагин для [Exteragram](https://exteragram.app/), который автоматически переводит исходящие сообщения в код Морзе. Любое сообщение можно декодировать обратно через контекстное меню.

### Возможности

- 🔡 **Автокодирование** — каждое отправляемое сообщение автоматически конвертируется в азбуку Морзе
- 🔍 **Декодирование по запросу** — удерживайте сообщение и выберите **«Decode»**, чтобы увидеть расшифровку
- 🌍 **Поддержка нескольких языков** — латиница, кириллица, цифры и основные знаки препинания
- ⚙️ **Переключатель** — кодирование можно включить или выключить в настройках плагина без удаления
- 🪖 **Режим NATO** — кодирование словами фонетического алфавита (Альфа, Браво, Чарли…) вместо точек и тире
- 🚫 **Защита от двойного кодирования** — уже закодированные сообщения не кодируются повторно

### Установка

Просто откройте файл плагина в **Exteragram**

### Использование

#### Отправка сообщения в коде Морзе
Просто напишите сообщение и нажмите **Отправить**. Плагин перехватит текст и переведёт его в азбуку Морзе (если кодирование включено в настройках).

Для ручного выбора режима используйте префиксы:
- `!m текст` — принудительно в Морзе
- `!n текст` — принудительно в NATO
- `!raw текст` — отправить без кодирования

#### Декодирование полученного сообщения
1. Удерживайте сообщение в коде Морзе
2. Выберите **«Decode»** в контекстном меню
3. В диалоге отобразится исходный код Морзе и расшифрованный текст

#### Настройки

| Параметр | Описание | По умолчанию |
|---|---|---|
| **Enable encoding** | Автоматически кодирует исходящие сообщения (Морзе или NATO) | ✅ Включено |
| **Prefix-only mode** | Кодировать только сообщения с префиксом `!m` или `!n` (без префикса — без кодирования; `!raw` — обход кодирования) | ❌ Выключено |
| **Default codec: NATO** | Использовать NATO (Альфа/Браво/Чарли) как кодек по умолчанию вместо Морзе | ❌ Выключено |
| **RU → NATO mode** | Транслитерировать русские буквы в латиницу перед кодированием в NATO (например, ПРИВЕТ → PRIVET → NATO) | ❌ Выключено |
| **Skip if already encoded** | Не кодировать сообщение повторно, если оно уже выглядит как Морзе или NATO | ✅ Включено |

### Таблица кодов

Плагин кодирует и декодирует **латиницу** (A–Z), **кириллицу** (А–Я), **цифры** (0–9) и множество знаков препинания:

```
. , ; : / ( ) ! ? _ " ' & - + = @ $
```

---

## 🇬🇧 English

An [Exteragram](https://exteragram.app/) plugin that automatically converts your outgoing messages to Morse code, with a built-in decoder accessible from the message context menu.

### Features

- 🔡 **Auto-encode** — every message you send is automatically converted to Morse code before delivery
- 🔍 **Decode on demand** — long-tap any message and choose **"Decode"** to see the decoded text in a dialog
- 🌍 **Multilingual support** — handles Latin letters, Cyrillic letters, digits, and common punctuation
- ⚙️ **Toggle switch** — enable or disable encoding from the plugin settings without uninstalling
- 🪖 **NATO mode** — encode messages using the phonetic alphabet (Alpha, Bravo, Charlie…) instead of dots and dashes
- 🚫 **Double-encoding protection** — already encoded messages are not encoded again

### Installation

Just open plugin file in **Exteragram**

### Usage

#### Sending a Morse-coded message
Just type your message and hit **Send** as usual. The plugin intercepts the message and converts it to Morse code automatically (when encoding is enabled in settings).

You can also use manual prefixes:
- `!m text` — force Morse encoding
- `!n text` — force NATO encoding
- `!raw text` — send without any encoding

#### Decoding a received message
1. Long-tap the Morse-coded message
2. Select **"Decode"** from the context menu
3. A dialog will show the original Morse and the decoded text

#### Settings

| Option | Description | Default |
|---|---|---|
| **Enable encoding** | Automatically encodes outgoing messages (Morse or NATO) | ✅ Enabled |
| **Prefix-only mode** | Only encode messages that start with `!m` or `!n` (use `!raw` to bypass encoding entirely) | ❌ Disabled |
| **Default codec: NATO** | Use NATO (Alpha/Bravo/Charlie) as the default codec instead of Morse | ❌ Disabled |
| **RU → NATO mode** | Transliterate Russian letters to Latin before NATO encoding (e.g. ПРИВЕТ → PRIVET → NATO) | ❌ Disabled |
| **Skip if already encoded** | Prevents double-encoding if the message already looks like Morse or NATO | ✅ Enabled |

### Morse code table

The plugin encodes/decodes **Latin** (A–Z), **Cyrillic** (А–Я), **digits** (0–9), and a wide range of punctuation and special characters:

```
. , ; : / ( ) ! ? _ " ' & - + = @ $
```
