# Foreword

Welcome to the official **Bot House** documentation! This guide is designed to help you quickly set up, manage, and build custom automated bots for both **Discord** and **Telegram**.

## What is Bot House?

Bot House is a powerful, visual, and scriptable bot creation platform. It allows users to build feature-rich bots across multiple messaging platforms using simple, intuitive functions—no complex backend setup or coding background required.

### Supported Platforms

- **Discord:** Create custom commands, auto-moderation, embeds, buttons, and event triggers.
- **Telegram:** Build custom command flows, interactive menus, inline queries, and multi-user chat bots.

---

## Key Features

- **Cross-Platform Support:** Deploy and manage bots on Discord and Telegram from a single platform.
- **Simple Functional Syntax:** Use readable, tag-based function signatures like `$title[...]`, `$description[...]`, and `$sendMessage[...]`.
- **Rich Embeds & Formatting:** Fully customize message appearance with titles, thumbnails, footer banners, and action components.
- **Built-in Hosting:** Manage your bots seamlessly with active hosting and built-in runtime tools.

---

## Quick Example

Here is a simple example showing how a basic command response works in Bot House:

```bdscript
$title[Welcome to Bot House!]
$description[Your bot is ready to serve both Discord and Telegram channels.]
$thumbnail[https://example.com/bot-house-logo.png]
$sendMessage[Hello world!]
```

---

## Navigation & Getting Started

- **[Quick Start Guide](discord/quickstart.md):** Learn how to connect your bot tokens and write your first command.
- **[Functions Reference](discord/overview.md):** Explore the complete list of supported scripting functions.
- **[API Reference](api/index.md):** Access the public API endpoints and JSON data schema.
