# 🌟 Xero 

Welcome to XeroLang.
This guide shows exactly how to write code that the current compiler can understand and successfully turn into Discord.js.

No extra features. No theory.
Just what works **right now**.

---

# 🚀 Step 1: Install XeroLang

Inside your XeroLang project folder:

```
npm install
npm link
```

This makes the `xero` command usable globally.

---

# 🔧 Step 2: Create Your First Xero File

Create:

```
bot.xero
```

Then add the code your compiler can parse:

```xero
bot "XeroBot" uses "YOUR_TOKEN"
intents: Guilds, GuildMessages, MessageContent

on ready:
    log "Bot is online."

command "ping":
    reply "pong!"

on message contains "help":
    send "Try saying ping!" to channel "general"
```

**Important:**
The compiler only understands single-line commands and indentation exactly like this.

---

# 🧰 Step 3: Compile Your Bot

Run:

```
xero bot.xero
```

If the script is valid, it generates:

```
output.js
```

This file contains the actual Discord.js bot code.

---

# ▶️ Step 4: Install Runtime Dependencies

```
npm install discord.js dotenv
```

Run your bot:

```
node output.js
```

---

# 📘 XeroLang Syntax (What the Compiler Actually Supports)

### ✔ Bot Declaration

```xero
bot "BotName" uses "TOKEN"
```

### ✔ Intents

```
intents: Guilds, GuildMessages, MessageContent
```

### ✔ Ready Event

```xero
on ready:
    log "message"
```

### ✔ Commands

```xero
command "ping":
    reply "pong!"
```

The compiler converts this into a message listener checking for exact match.

### ✔ Message Contains Trigger

```xero
on message contains "word":
    send "text" to channel "general"
```

### ✔ Send a Message to a Channel

```xero
send "TEXT" to channel "CHANNEL_NAME"
```

### ✔ Slash Commands (Declared Only)

```xero
slash "name" description "text":
    reply "something"
```

(Slash commands are collected but not registered automatically.)

---

# ❗ Features That DO NOT Work (Yet)

The current compiler **does NOT** support:

* Variables
* Math (`+=`, `=`, etc.)
* Token blocks (`token "..."`)
* Arrow syntax (`send -> channel`)
* Events other than:

  * `on ready`
  * `on message contains`
* Multiline replies
* Nested structures
* Logic (if/else)
* Role management
* Loops
* Imports




