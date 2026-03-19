---
id: create-chatbot
slug: /chat
title: Create & Manage Chatbots
sidebar_position: 1
---

import createbot from '/img/chat/create-new.png';
import switchbot from '/img/chat/switch-bots.png';
import renamebot from '/img/chat/rename-bot.png';
import chatbotsettings from '/img/chat/chatbot-settings.png';
import shortcodepill from '/img/chat/shortcode-pill.png';
import shortcodeinsert from '/img/chat/shortcode-insert.png';
import popupenable from '/img/chat/popup-enable.png';
import popupsettings from '/img/chat/popup-settings.png';
import embedenable from '/img/chat/embed-enable.png';
import embedcode from '/img/chat/embed-code.png';
import chatui from '/img/chat/chat-ui.png';

# Create & Manage Chatbots

You can deploy chatbots in three ways:

- **On-page**: Embed the chatbot directly inside a page, post, or widget with a shortcode.
- **Popup**: Show the chatbot as a floating launcher on your site.
- **Embed Anywhere**: Add the chatbot to an external website with a script snippet.

This guide covers the current chatbot builder UI and the basic workflow for creating, managing, and deploying bots.

👉 Check out the live demo here: [aipower.org/demo](https://aipower.org/demo)

## Create a New Chatbot

1. Navigate to **AI Puffer > Chat**.
2. Click the **+** button in the chatbot tab row.

<img src={createbot} width="600" />

3. A new bot is created immediately with the default name **New Chatbot**.
4. Use the **Name** field in the **Chatbot** accordion to rename it.

<img src={renamebot} width="600" />

## Switch and Manage Bots

Every install includes a **Default Bot** to help you get started.

- Use the chatbot tabs at the top of the builder to switch between bots.
- If you have many bots, extra bots move into the overflow list.

<img src={switchbot} width="600" />

- The current bot’s shortcode is shown in a pill at the top. Click it to copy.
- Open the **Actions** accordion to **Duplicate**, **Reset**, or **Delete** the active bot.

<img src={chatbotsettings} width="600" />

The **Default Bot** cannot be deleted.

## Deploy Your Chatbot

The top area of the builder controls deployment. It includes the shortcode pill, the **Mode** dropdown, and the **Site-Wide** option when popup mode is selected.

### On-page

1. Select **On-page** in the **Mode** dropdown.
2. Click the shortcode pill to copy it.

<img src={shortcodepill} width="600" />

3. Paste the shortcode into any page, post, or widget.

Example:

```shortcode
[aipkit_chatbot id=9453]
```

<img src={shortcodeinsert} width="600" />

### Popup

1. Select **Popup** in the **Mode** dropdown.
2. Choose whether the popup should be **Site-Wide** or only used where the bot is embedded.

<img src={popupenable} width="600" />

3. Open the **Appearance** accordion to customize the launcher, icon, avatar, greeting, popup hint, and other UI details.

Popup-specific options include launcher position, shape, size, delay, hint behavior, and status text.

### Embed Anywhere (External Sites)

Select **Embed Anywhere** in the **Mode** dropdown to open the setup modal.

<img src={embedenable} width="600" />

1. Copy the generated embed code.
2. Add the external domains you want to allow, one URL per line.

<img src={embedcode} />

3. Paste the snippet into the external site’s HTML, usually before the closing `</body>` tag.

## The Chatbot Builder

The builder has two main columns:

- **Left column**: bot tabs, deployment controls, and all chatbot settings.
- **Right column**: preview of the active chatbot.

<img src={chatui} />

Settings are organized into accordions:

- **Chatbot**: Name, Engine, Model, and Instructions.
- **Context**: Choose data sources such as **Page Context** and **Vector**. When Vector is enabled, the **Training Data** panel appears with tabs for **Q&A**, **Text**, **Files**, and **Website** content.
- **Tools**: Enable features like file upload, web search, image analysis, image generation, speech-to-text, text-to-speech, and realtime voice.
- **Behaviour**: Configure streaming, session memory, creativity, response length, memory depth, and reasoning.
- **Appearance**: Control theme, launcher, greetings, placeholder text, footer, typing text, conversation starters, sidebar, fullscreen, feedback, copy, and download.
- **Rules**: Create rule-based automations for chatbot events and actions. See [Triggers](./triggers.md).
- **Connected Apps**: View and manage app connections for the selected chatbot.
- **Safety**: Configure IP anonymization, moderation, consent notice, banned words, and blocked IPs.
- **Limits**: Set general or role-based token limits, reset period, and the message shown when a limit is reached.
- **Actions**: Duplicate, reset, or delete the current bot.

Some sections include **Edit** or **Configure** buttons that open flyouts or sheets for advanced settings.

For more detail on specific areas, see:

- [AI Configuration](./ai-configuration.md)
- [Context](./context.md)
- [Appearance](./appearance.md)
- [Image Features](./image-features.md)
- [Voice Features](./voice-features.md)
- [Security & Privacy](./security-privacy.md)
- [Token Management](./token-management.md)

## Saving Changes

Chatbot settings save automatically after you change them. You will see a saving status in the builder header while updates are being stored.