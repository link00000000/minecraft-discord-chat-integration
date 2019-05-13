# minecraft-discord-chat-integration
Bridges the chat between minecraft ingame server and a discord channel

## How it works
All commands are polled through rcon and are parsed for a message sent by a player. If the message is sent by a player, that message is then relayed to a specific channel on a discord server. Furthermore, if a message is sent in that channel on discord, the message is replayed back and displayed on the server though rcon.

## Setup
1. Enable rcon in server.properties and set a password. Be sure to portforward the port used by minecraft's rcon (defualt: 25575)
2. Edit config.json
3. run `npm install` to install all required npm packges
4. run `npm start` to start the bridge between rcon and discord
