# Nami Assistant Website

A static, GitHub Pages-ready personal-assistant experience with a Y2K computer aesthetic. It has no backend, no API key, and no external data storage beyond the browser’s `localStorage`.

## Features

- Chat interface, history persistence, CRT scanlines, desktop window chrome, and responsive layout.
- Voice input through the Web Speech API when supported; clear in-app fallback notice when it is not.
- Optional spoken replies through browser text-to-speech.
- Local preference and correction memory. Use phrases such as `remember that I prefer concise answers`, or use **CORRECT / TEACH NAMI** on any Nami reply.
- Explainable Learning Cache panel, JSON export, clear chat, and reset-memory controls.

Nami does **not** train a model. It saves small local notes and uses them to shape future on-page responses in the same browser.

## Run locally

## Capability boundary

Nami can launch a web search when you type or say `search the web for ...`. This static version cannot read webpages for you, access your accounts, send messages, or perform unrestricted web actions. Those features require a secure hosted backend plus explicitly authorized integrations.

For speech, Nami prefers a friendlier, feminine-sounding installed browser voice (for example Zira or Samantha) when one is available. The exact available voice is controlled by the device and browser.

Open `index.html` in a modern browser. Voice input often requires HTTPS or localhost, so it works most reliably once deployed to GitHub Pages.

## Publish with GitHub Pages

1. Create a new GitHub repository, for example `nami-assistant`.
2. Upload the contents of this folder (not the folder itself) to the repository root and commit.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
5. After GitHub publishes it, open the Pages URL shown there. GitHub Pages serves HTTPS, which is needed by many browsers for microphone access.

## Browser support

Chat and local learning work in any modern browser with localStorage. Speech recognition support is strongest in Chromium-based browsers and can vary by browser/device. Text-to-speech has broader support. The interface stays usable when either feature is unavailable.
