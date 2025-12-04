# XeroLang Changelog

## 1.0.0 – Current Version
- Added support for basic bot declaration:
  - `bot "NAME" uses "TOKEN"`
  - `intents: ...`
- Implemented simple event handling:
  - `on ready`
  - `on message contains "TEXT"`
- Added command system:
  - `command "NAME":`
  - `reply "TEXT"`
- Added message-sending syntax:
  - `send "TEXT" to channel "CHANNEL"`
- Added basic slash command declarations:
  - `slash "NAME" description "DESC"`
  - (Declaration only; registration not automated.)
- Implemented line-based tokenizer and parser.
- Implemented JS generator that outputs `output.js` using Discord.js v14.
- Added CLI to compile files:
  - `xero <file.xero>`
- Added simple example `.xero` file for beginners.
- Added VS Code extension with highlighting, snippets, and language config.

