# Morsegram — Exteragram Plugin

---

## 🇷🇺 Русский

Плагин для [Exteragram](https://exteragram.app/), который автоматически переводит исходящие сообщения в код Морзе. Любое сообщение можно декодировать обратно через контекстное меню.

### Возможности

- 🔡 **Автокодирование** — каждое отправляемое сообщение автоматически конвертируется в азбуку Морзе
- 🔍 **Декодирование по запросу** — удерживайте сообщение и выберите **«Decode Morse»**, чтобы увидеть расшифровку
- 🌍 **Поддержка нескольких языков** — латиница, кириллица, цифры и основные знаки препинания
- ⚙️ **Переключатель** — кодирование можно включить или выключить в настройках плагина без удаления

### Требования

| | |
|---|---|
| Exteragram | ≥ 11.12.0 |

### Установка

1. Откройте **Exteragram → Настройки → Exteragram → Плагины**
2. Нажмите **+** и выберите файл `morse_code.plugin`
3. Включите плагин — готово!

### Использование

#### Отправка сообщения в коде Морзе
Просто напишите сообщение и нажмите **Отправить**. Плагин перехватит текст и переведёт его в азбуку Морзе (если кодирование включено в настройках).

#### Декодирование полученного сообщения
1. Удерживайте сообщение в коде Морзе
2. Выберите **«Decode Morse»** в контекстном меню
3. В диалоге отобразится исходный код Морзе и расшифрованный текст

#### Настройки
| Параметр | Описание | По умолчанию |
|---|---|---|
| Encode outgoing messages | Автоматически конвертирует исходящие сообщения в азбуку Морзе | ✅ Включено |

### Таблица кодов

Плагин кодирует и декодирует **латиницу** (A–Z), **кириллицу** (А–Я), **цифры** (0–9) и множество знаков препинания:

```
. , ; : / ( ) ! ? _ " ' & - + = @ $
```

### Автор

**@fiudeus**

### Лицензия

Плагин предоставляется «как есть». Используйте на свой страх и риск.

---

## 🇬🇧 English

An [Exteragram](https://exteragram.app/) plugin that automatically converts your outgoing messages to Morse code, with a built-in decoder accessible from the message context menu.

### Features

- 🔡 **Auto-encode** — every message you send is automatically converted to Morse code before delivery
- 🔍 **Decode on demand** — long-tap any message and choose **"Decode Morse"** to see the decoded text in a dialog
- 🌍 **Multilingual support** — handles Latin letters, Cyrillic letters, digits, and common punctuation
- ⚙️ **Toggle switch** — enable or disable encoding from the plugin settings without uninstalling

### Requirements

| | |
|---|---|
| Exteragram | ≥ 11.12.0 |

### Installation

1. Open **Exteragram → Settings → Exteragram → Plugins**
2. Tap the **+** button and choose `morse_code.plugin`
3. Enable the plugin — that's it!

### Usage

#### Sending a Morse-coded message
Just type your message and hit **Send** as usual. The plugin intercepts the message and converts it to Morse code automatically (when encoding is enabled in settings).

#### Decoding a received message
1. Long-tap the Morse-coded message
2. Select **"Decode Morse"** from the context menu
3. A dialog will show the original Morse and the decoded text

#### Settings
| Option | Description | Default |
|---|---|---|
| Encode outgoing messages | Automatically converts your messages to Morse code before sending | ✅ Enabled |

### Morse code table

The plugin encodes/decodes **Latin** (A–Z), **Cyrillic** (А–Я), **digits** (0–9), and a wide range of punctuation and special characters:

```
. , ; : / ( ) ! ? _ " ' & - + = @ $
```

### Author

**@fiudeus**

### License

This plugin is provided as-is. Use at your own risk.
