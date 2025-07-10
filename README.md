Discord Support Bot for Remote Assistance
This bot system allows you to send commands directly to support clients (user PCs) via a Discord bot—no need to host your own backend server. Clients communicate with the Discord bot through direct messages (DMs).

Features
Device identification via HWID

Send commands to individual devices (e.g., add antivirus exclusions)

Clients actively fetch commands from the bot

Clients send status updates, posted in a designated Discord admin channel

Full control and transparency through Discord

No separate backend server required

How it works
Discord Bot:

Receives commands from you via Discord chat (!sendcmd <HWID> <command>)

Stores commands and delivers them to clients

Receives client status updates and posts them in the admin channel

Support Client (Python script on user PCs):

Identifies itself with HWID to the bot

Periodically fetches new commands via DM

Executes commands (e.g., setting antivirus folder exclusions)

Sends execution results back to the bot

Requirements
Discord bot token and admin channel ID

Python 3 installed on client machines

User permission to run the support tool with admin rights (needed for some commands)

Installation & Usage
Create a Discord bot and insert its token into bot.py

Run the client script on the target machines

Send commands to devices via Discord chat

Monitor status updates live in the Discord admin channel

Support
If you have questions or want to add features, feel free to reach out!

