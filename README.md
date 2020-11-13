# twitch-permit-bot

## Setup
Clone repository: `git clone git@github.com:EchtkPvL/twitch-permit-bot.git`

Change directory: `cd twitch-permit-bot/`

Install needed modules: `npm install`

Copy `config.js.example` to `config.js` and insert credentials.

Start Bot: `node index.js`

## Known issues
```
TypeError: Cannot read property 'resolveNs' of undefined
    at check_link (/home/echtkpvl/twitch-mybot/index.js:151:34)
    at client.on (/home/echtkpvl/twitch-mybot/index.js:72:9)
    at client.EventEmitter.emit (/home/echtkpvl/twitch-mybot/node_modules/tmi.js/lib/events.js:101:25)
    at client.EventEmitter.emits (/home/echtkpvl/twitch-mybot/node_modules/tmi.js/lib/events.js:64:19)
    at client.handleMessage (/home/echtkpvl/twitch-mybot/node_modules/tmi.js/lib/client.js:1003:34)
    at parts.forEach (/home/echtkpvl/twitch-mybot/node_modules/tmi.js/lib/client.js:1080:36)
    at Array.forEach (<anonymous>)
    at client._onMessage (/home/echtkpvl/twitch-mybot/node_modules/tmi.js/lib/client.js:1079:11)
    at WebSocket.onMessage (/home/echtkpvl/twitch-mybot/node_modules/ws/lib/event-target.js:120:16)
    at emitOne (events.js:116:13)
```
Fix: Update NodeJS (I'm using v14.15.0)
