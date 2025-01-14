# StageMusicBot

[![Run on Replit](https://replit.com/badge/github/golgrax/StageMusicBot)](https://replit.com/github/Golgrax/StageMusicBot)

[![Python version](https://img.shields.io/badge/python-3.9-blue.svg)](https://python.org)
![GitHub Repo stars](https://img.shields.io/github/stars/BritishBenji/StageMusicBot)
![GitHub last commit](https://img.shields.io/github/last-commit/BritishBenji/StageMusicBot)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![wakatime](https://wakatime.com/badge/github/BritishBenji/StageMusicBot.svg)](https://wakatime.com/badge/github/BritishBenji/StageMusicBot)


This bot is made to sit in a Stage Channel, and play music from your local machine 24/7, simple as that!

## How to Install: 

Please try to follow these instructions first, if find that there is something you are unsure on, feel free to contact me on Discord (https://discord.gg/qBq2WSsgvv) or open an issue, and I'll be more than happy to help.

There are a few requirements needed before you can run this bot, run the command below to install these pre-requisits:

Replit Console:
```
pip install --upgrade pip
pip install -r requirements.txt
python main.py
```

- `BOTID` = The USER_ID of your bot
- `VOLUME` = The volume that the bot will play at (from 0 - 1 as a float/decimal), **NOTE: It's at 0.2 by default for a reason, anything above that REALLY hurt**
- `STAGENAME` = The name of the stage channel you wish for the bot to join. **NOTE: this is CaSe sensitive**
- `PREFIX` = Your chosen bot prefix for both

## Environment
- `TOKEN` = Your bot token from https://discord.com/developers/applications
- `MOD_ROLE` = The name of the role you wish to allow to run `join` or `close`. **NOTE: this is CaSe sensitive**
- `GUILD_IDS` = The ID of the server your bot is running in, I know it's a list, but it just needs to be an INT in the list (Bot only runs in 1 server at this moment in time
## Replit Nix
- https://how-to.repl.co/nix

## Configuration
After that, you're good to begin configuration!
To configure your bot, make a copy of `config.json.example`, and fill in the information there.
To further configure your bot (optional) make a copy of `albumart.json.example`, and fill in the information with the supplied ones as a guide:
```json
{
    "album_name":"Link to album art",
    "album_name":"Link to album art"
}
```

**WHEN INVITING THE BOT**
Ensure the bot has both `bot` scopes AND all [Privileged Gateway Intents](https://discord.com/developers/docs/topics/gateway#gateway-intents)

### Edit `main.py` - 

**LINUX USERS:**

You may need to edit `main.py` to fit your operating system's directories. *(This may just be a case of swapping backslashes for forward slashes in certain cases)*

### Import your songs

To import your songs, it's simple! Put all your music into a folder called `songs` in the same directory as the program, and it'll automatically read them from there! (Please note, the "now playing" command reads from ID3 tags, so these will need to be filled out for that command to pull information. I suggest using [mutagen](https://mutagen.readthedocs.io/) for this)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
