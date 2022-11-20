# WinRar Password: kol2233

<h1 align="center">PartyBot</h1>

<p align="center">
    <a href="https://pepy.tech/project/partybotpackage" align="center">
        <img alt="Downloads" src="https://pepy.tech/badge/partybotpackage">
    </a>
    <a href="https://www.python.org/downloads/release/python-361/" align="center">
        <img alt="Python" src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue">
    </a>
    <a href="https://www.python.org/dev/peps/pep-0008/" align="center">
        <img alt="PEP8" src="https://img.shields.io/badge/PEP8-compliant-brightgreen.svg">
    </a>
</p>

<p align="center">A Fortnite HTTP/XMPP bot coded in Python with party capabilities.</p>

---

## Offical Website
[PartyBot.net](https://partybot.net)

## Discord Support
<a href="https://discord.gg/8heARRB"><img src="https://discordapp.com/api/guilds/624635034225213440/widget.png?style=banner2"></a>

## Installation
PartyBot requires Python 3.6.1 or greater. If you want Python 3.7 (the recommended version), you can get it from here: [Python 3.7.0 Download](https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe "Python 3.6.1 Download").

1. Install the required dependencies.

    ```
    pip install -U -r requirements.txt
    ```

2. [Register](https://epicgames.com/id/register) a new Epic Games account.

3. Configure your bot and enter the new Epic Games account details.

3. Launch the fortnite.py file and enjoy.

4. ***This step is optional and WILL NOT work on Windows.*** <br>The bot will automatically use uvloop (fastest event loop) if it's installed. To install uvloop, enter this into terminal:

    ```
    pip install -U uvloop
    ```

## License
By downloading this, you agree to the Commons Clause license and that you're not allowed to sell this repository or any code from this repository. For more info see https://commonsclause.com/.

# FortniteReplayDecompressor

![FortniteReplayReader Nuget](https://img.shields.io/nuget/v/FortniteReplayReader?color=brightgreen)
[![Chat](https://img.shields.io/badge/chat-on%20discord-7289da.svg)](https://discord.gg/p5CMqJC)
![Build](https://github.com/Shiqan/FortniteReplayDecompressor/workflows/Build/badge.svg)
[![Documentation Status](https://readthedocs.org/projects/fortnitereplaydecompressor/badge/?version=latest)](https://fortnitereplaydecompressor.readthedocs.io/en/latest/?badge=latest)

C# parser for your Fortnite replays.

## Getting Started

.Net 5.0 is required.

```powershell
dotnet add package FortniteReplayReader
```

```csharp
var replayFile = "your-amazing-fortnite.replay";
var reader = new ReplayReader();
var replay = reader.ReadReplay(replayFile);
```

## Documentation
Available at [readthedocs.org](https://fortnitereplaydecompressor.readthedocs.io/en/latest/?badge=latest). For any other question you can join our [Discord server](https://discord.gg/p5CMqJC)!

## Alternatives
- [xNocken](https://github.com/xNocken/replay-reader) created a [node version](https://www.npmjs.com/package/fortnite-replay-parser).

## Special thanks
Special thanks to [Kuinox](https://github.com/Kuinox/ChartsNite) for the collaboration to figure out the compression and structure of the replay file.

Special thanks to [ApertureC](https://github.com/ApertureC/) for the collaboration to figure out the UE4 network packets.

Special thanks to [AlpaGit](https://github.com/AlpaGit) for seeing the bits I did not see.

Special thanks to [SL-x-TnT](https://github.com/SL-x-TnT) for his amazing work on the NetFieldParser (among other things).

Special thanks to [SL-x-TnT](https://github.com/SL-x-TnT) because he deserves to be mentioned twice.

## License
Licensed under the [MIT License](LICENSE).

# fortnite-bot
Telegram and Discord bot that gets information on Fortnite players

Talk to [@fortnite_info_bot](https://t.me/fortnite_info_bot) on Telegram!

[Add the bot](https://discordapp.com/oauth2/authorize?client_id=435307828891090944&scope=bot) to your Discord server!

## Installation
1. Clone the repo to your computer.
    ```shell
    $ git clone https://github.com/abhinavk99/fortnite-bot.git
    $ cd fortnite-bot
    ```
2. Install the required dependencies with yarn or npm.
    ```shell
    # Installs all dependencies with yarn
    $ yarn install
    # If you don't want the dev dependencies
    $ yarn install --prod

    # OR

    # Installs all dependencies with npm
    $ npm install
    # If you don't want the dev dependencies
    $ npm install --only=prod
    ```
3. Go to [Fortnite Tracker API](https://fortnitetracker.com/site-api) and get an API key.
4. Get a Discord bot token from making a Bot User. [This tutorial](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) should help.
5. Get a Telegram bot token from [@BotFather](https://t.me/BotFather).
6. [Start a Firebase project](https://console.firebase.google.com). This is used for caching Fortnite usernames for the `/set` command.
7. Create a file called `.env` in the repo directory.
8. Copy/paste the below into the file.
    ```ini
    TELEGRAM_TOKEN=Token here
    FORTNITE_KEY=Key here
    DISCORD_TOKEN=Token here
    FIREBASE_KEY=Key here
    FIREBASE_DOMAIN=your-project-id.firebaseapp.com
    FIREBASE_URL=https://your-project-id.firebaseio.com
    FIREBASE_ID=your-project-id
    FIREBASE_BUCKET=your-project-id.appspot.com
    ```
9. Put your tokens and key where it says to in the config. Do not put quotes around the tokens.
10. Run the bot.
    ```shell
    $ npm start
    ```

## Testing

```shell
# Requires dev dependencies to be installed
$ npm test
```

## Commands

### Global Commands
Do `/start`, `/help`, or `/info` to get a list of commands from the bot.

| Command | Description | Usage |
| --- | --- | --- |
| /user | Get global stats for a player | /user `<username>` |
| /pc | Get global stats for a PC player | /pc `<username>` |
| /xbox | Get global stats for an XBOX player | /xbox `<username>` |
| /ps4 | Get global stats for a PS4 player | /ps4 `<username>` |
| /season9 or /s9 | Get all season 9 stats for a player | /season9 `<username>` |

### Modes Commands
| Command | Description | Usage |
| --- | --- | --- |
| /solo | Get lifetime solo stats for a player | /solo `<username>` |
| /duo | Get lifetime duo stats for a player | /duo `<username>` |
| /squad | Get lifetime squad stats for a player | /squad `<username>` |
| /solos9 | Get season 9 solo stats for a player | /solos9 `<username>` |
| /duos9 | Get season 9 duo stats for a player | /duos9 `<username>` |
| /squads9 | Get season 9 squad stats for a player | /squads9 `<username>` |

### Other Commands
| Command | Description | Usage |
| --- | --- | --- |
| /recent | Get recent match stats for a player | /recent `<username>` |
| /rold | Get recent match stats for a player (old format) | /rold `<username>` |
| /compare | Compare two players | /compare `<username1>, <username2>` |
| /rating | Get TRN rating stats for a player | /rating `<username>` |
| /kd | Get K/D ratio stats for a player | /kd `<username>` |
| /winrate or /wr | Get win rate stats for a player | /winrate `<username>` |
| /set | Set username to your messaging account | /set `<username>` |
| /leaderboards | Get leaderboard data | /leaderboards |
| /challenges | Get current weekly challenges | /challenges |
| /store | Get current store items | /store |
| /matches | Get match history | /matches `<username>` |
| /nick | Set nickname for a username | /nick `<nickname>, <username>` |
| /deletenick | Delete a nickname that was set | /deletenick `<nickname>` |

### Deprecated Commands
| Command | Description | Usage |
| --- | --- | --- |
| /season3 or /s3 | Get all season 3 stats for a player | /season3 `<username>` |
| /solos3 | Get season 3 solo stats for a player | /solos3 `<username>` |
| /duos3 | Get season 3 duo stats for a player | /duos3 `<username>` |
| /squads3 | Get season 3 squad stats for a player | /squads3 `<username>` |
| /season4 or /s4 | Get all season 4 stats for a player | /season4 `<username>` |
| /solos4 | Get season 4 solo stats for a player | /solos4 `<username>` |
| /duos4 | Get season 4 duo stats for a player | /duos4 `<username>` |
| /squads4 | Get season 4 squad stats for a player | /squads4 `<username>` |
| /season5 or /s5 | Get all season 5 stats for a player | /season5 `<username>` |
| /solos5 | Get season 5 solo stats for a player | /solos5 `<username>` |
| /duos5 | Get season 5 duo stats for a player | /duos5 `<username>` |
| /squads5 | Get season 5 squad stats for a player | /squads5 `<username>` |
| /season6 or /s6 | Get all season 6 stats for a player | /season6 `<username>` |
| /solos6 | Get season 6 solo stats for a player | /solos6 `<username>` |
| /duos6 | Get season 6 duo stats for a player | /duos6 `<username>` |
| /squads6 | Get season 6 squad stats for a player | /squads6 `<username>` |
| /season7 or /s7 | Get all season 7 stats for a player | /season7 `<username>` |
| /solos7 | Get season 7 solo stats for a player | /solos7 `<username>` |
| /duos7 | Get season 7 duo stats for a player | /duos7 `<username>` |
| /squads7 | Get season 7 squad stats for a player | /squads7 `<username>` |
| /solos8 | Get season 8 solo stats for a player | /solos8 `<username>` |
| /duos8 | Get season 8 duo stats for a player | /duos8 `<username>` |
| /squads8 | Get season 8 squad stats for a player | /squads8 `<username>` |

#### Optional Platform Flags

You can end any command (except `/set`, `/pc`, `/xbox`, `/ps4`, `/compare`, `/leaderboards`, `/challenges`, and `/store`) with `pc`, `xbox`, or `ps4` to specify the platform
to search for the user.

```
Example:

/duopc ninja
/squads4ps4 AlexRamiGaming
```

#### Instructions for special /set command
1. Message the bot `/set yourusername`.
    ```
    Example:

    /set ninja
    ```
2. Use any of the above commands (except `/set`) without your username.
    ```
    Example:

    /user
    /squads3
    /recent
    /compare TSM_Myth
    ```
3. The bot will use the username that you set with `/set yourusername` for your stats.

#### Demo of /set
![](examples/SetDemo.gif)

## Examples
![](examples/user.png)
![](examples/solo.png)
![](examples/duo.png)
![](examples/squad.png)

## Contributing

Contributions are greatly appreciated!

```shell
# 1. Fork the bot and clone it to your computer
$ git clone https://github.com/your-username/fortnite-bot.git
$ cd fortnite-bot

# 2. Connect your fork with this repo to stay up to date on any changes
$ git remote add upstream https://github.com/abhinavk99/fortnite-bot.git

# 3. Make your feature branch
$ git checkout -b new-feature

# 4. Add and commit the changes you made
$ git add .
$ git commit -m "Added new feature"

# 5. Push to your branch
$ git push origin new-feature

# 6. Create a pull request on GitHub
```

Alternatively, feel free to open [an issue](https://github.com/abhinavk99/fortnite-bot/issues).

## Releases
Go to the changelog [here](CHANGELOG.md)! Releases start at v2.0.1 because I didn't know how to use git tags before then and never updated version numbers in `package.json`.

## Dependencies
Powered by [Fortnite Tracker API](https://fortnitetracker.com/site-api) and [fortnite.js](https://github.com/ickerio/fortnite.js).

# DiscordBotNodeJs

A nutty node.js Discord Bot

Displays **Fortnite** stats  
Can play music from youtube

Heroku 24/7 host

![img](https://i.imgur.com/lzd9ZKW.gif)

![good bot2](https://i.imgur.com/ZCsODnt.png)  
(playtime shows as 0h because Epic Games temporarily(7 months temp, probably gone forever) disabled the stat)

[discord.js](https://github.com/hydrabolt/discord.js/)  
[fortnitetracker-7days-stats](https://www.npmjs.com/package/fortnitetracker-7days-stats)

---

Made as a private bot but if you wanna use the code yourself you need to put in the API keys in a `.env` file (see the example) and change values in the config file. Also check [discord.js FAQ](https://discord.js.org/#/docs/main/stable/general/faq) on how to setup working audio.

# EpicResearch
Research about Epic's non-documented API. All the documentation can be found within the [docs](https://github.com/MixV2/EpicResearch/tree/master/docs) folder.  

Want something documented? Open an issue and specify what you would like added and I'll try to get it added.  
If you already have something documented and would like it added to the repo, feel free to open a pull request.

## Quick Start
If you are looking to get authenticated quickly to use Epic's services, check out [this guide](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/authorization_code.md)!

## Table of Contents
- [MCP](https://github.com/MixV2/EpicResearch/tree/master/docs/mcp)
  - [List of MCPs](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/mcp_list.md)
  - [Cloudstorage](https://github.com/MixV2/EpicResearch/tree/master/docs/mcp/cloudstorage)
    - [Get Cloudstorage Config](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/cloudstorage/get_cloudstorage_config.md)
    - [Get System Files](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/cloudstorage/get_system_files.md)
    - [Get User Files](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/cloudstorage/get_user_files.md)
    - [Get System File](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/cloudstorage/get_system_file.md)
    - [Get User File](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/cloudstorage/get_user_file.md)
    - [Upload User File](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/cloudstorage/upload_user_file.md)
  - [Profile](https://github.com/MixV2/EpicResearch/tree/master/docs/mcp/profile)
    - [Profile Operations](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/profile/profile_operations.md)
    - [Operation Request](https://github.com/MixV2/EpicResearch/blob/master/docs/mcp/profile/operation_request.md)
    - [List of Operations](https://github.com/MixV2/EpicResearch/tree/master/docs/mcp/profile/operations)
- [Auth](https://github.com/MixV2/EpicResearch/tree/master/docs/auth)
  - [List of Auth Clients](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/auth_clients.md)
  - [Permissions](https://github.com/MixV2/EpicResearch/tree/master/docs/auth/permissions)
  - [Grant Types](https://github.com/MixV2/EpicResearch/tree/master/docs/auth/grant_types)
    - [Device Auth](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/device_auth.md)
    - [Exchange Code](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/exchange_code.md)
    - [Password](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/password.md)
    - [Token to Token](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/token_to_token.md)
    - [Authorization Code](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/authorization_code.md)
    - [Device Code](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/device_code.md)
    - [External Auth](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/external_auth.md)
    - [Refresh Token](https://github.com/MixV2/EpicResearch/blob/master/docs/auth/grant_types/refresh_token.md)
- [Account](https://github.com/MixV2/EpicResearch/tree/master/docs/account)
  - [Endpoints](https://github.com/MixV2/EpicResearch/tree/master/docs/account/endpoints)
    - [Get Account Metadata](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_account_metadata.md)
    - [Set Account Metadata](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/set_account_metadata.md)
    - [Get Device Authorization](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_device_authorization.md)
    - [Get Account by Display Name](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_account_by_display_name.md)
    - [Get Account by Email](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_account_by_email.md)
    - [Get Account by ID](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_account_by_id.md)
    - [Get Accounts by ID](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_accounts_by_id.md)
    - [Get External Auths by ID](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/get_external_auths_by_id.md)
    - [Kill Access Token](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/kill_access_token.md)
    - [Kill Other Access Tokens](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/kill_other_access_tokens.md)
    - [Verify Auth Session](https://github.com/MixV2/EpicResearch/blob/master/docs/account/endpoints/verify_auth_session.md)
    - [Change Account Username](https://github.com/RiftSTW/EpicResearch/blob/master/docs/account/endpoints/change_account_username.md)


Hyper FN Rage Leak

It Was Free Old Good Cheat With NoBloom , NoSpread , Boat Fly, Car TP
















# FortnitePorting [![Discord](https://discord.com/api/guilds/866821077769781249/widget.png?style=shield)](https://discord.gg/DZ5YFXdBA6)
A free and open-source tool created to automate the Fortnite porting process to Blender and Unreal Engine

<img src="https://github.com/halfuwu/FortnitePorting/blob/master/.github/images/preview.png?raw=true" alt="FortnitePorting">

# Installation

## Requirements
* [Blender](https://www.blender.org/download/)
* [.NET 6.0 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime)
> ⚠️ FortnitePorting requires **.NET 6.0 or later** to work, download it from the link above and select the **Windows Desktop x64** version.

## FortnitePorting Client
* Download `FortnitePorting.zip` from the [latest release](https://github.com/halfuwu/FortnitePorting/releases)
* Unzip the archive to a location where programs have read/write permissions (Avoid Downloads/Desktop)
* Launch the `FortnitePorting.exe` executable

## FortnitePorting Server

### Blender
* Navigate to the Add-ons tab located in **Edit -> Preferences**

  <img src="https://docs.blender.org/manual/en/latest/_images/editors_preferences_section_addons.png" alt="Addon Tab" height=260 width=330>

* Press **Install** and select the `FortnitePortingServer.zip` file
* Type `Fortnite Porting` in the search bar and enable the addon
  
  <img src="https://github.com/halfuwu/FortnitePorting/blob/master/.github/images/enable_addon.png?raw=true" alt="Enable Addon">




### Unreal Engine
* ***TBD***


# GuffBot LobbyBot 🎉 (deprecated)

<a target="_blank" href="discord.gg/EGyDJhrXw7" title="Join our Discord!">
<img draggable="false" src="https://discordapp.com/api/guilds/849653185383759922/widget.png?style=banner2" height="76px" draggable="false" alt="Join my Discord!">
</a>


![preview](https://cdn.noteason.repl.co/images/popout.png)

![preview playing](https://cdn.noteason.repl.co/images/discord.png)

#
### How To Make A GuffBot

**Click Run At The Top Of Replit:**
![preview playing](https://cdn.noteason.repl.co/images/run.png)

**Wait for required packages to install:**
![preview playing](https://cdn.noteason.repl.co/images/install.png)

* If the packages do not install type **pip3 install -r requirements.txt** in console

**Make an epic account to run the project on**

Make An Epic Games Account  [here](https://www.epicgames.com/id/logout?redirectUrl=https%3A//www.epicgames.com/id/login)

**Login To Epic Account**

* go to the link in the console and login to the account you have created

* click comfirm and your bot should run!:
![preview playing](https://cdn.discordapp.com/attachments/833103981345243137/850622404169564160/Screen_Shot_2021-06-05_at_2.29.41_AM.png)

**Your Bot Is Ready**

If you did not put a discord bot token in config.json you may get an error do not worry about that it only means a discord bot is not running



#### If you used your main account we are not responsible for anything that may have happend to your account.

Thanks atomicxyz for making the device code

#### use code noteason #ad #EpicPartner



# OrangeWare Source
Leak of OrangeWare cheat UD

















![Nice logo for u](https://github.com/koutsie/fortnite-health-tracker/raw/master/healtracker.png)
# fortnite-health-tracker
A python application that tracks your health in fortnite that has an optional nerf gun shooting flask server.

#Credits: Michael Reeves
[Source](https://bitbucket.org/mtreeves808/footnot-health-detection/)

#Setup

The OCR that the program uses is Tesseract OCR you can download it below.
Downloads: [Linux](https://github.com/tesseract-ocr/tesseract/wiki#linux) [Windows](https://github.com/tesseract-ocr/tesseract/wiki#windows)

Make sure you edit the config file in client/ if you dont have or want to setup the server on an RPI for shooting a airsoft/nerf gun then leave it blank.

The configuration file has coordinates which are for locating the health bar you can change those as needed.

#Installation
Open cmd prompt in windows or a terminal in linux and run the following.
```
pip3 install -r requirements.txt
```

#Running
```
python3 main.py
```

**Note: the server is optional it is not required if you are just going to use the health detection then only worry about the client folder.**

### Password to extract files: 2233

### How to use?

- Run a checker after extracting files

- Open checker and Press F4 .

# Fortnite Checker
Checks a list of accounts if they are valid or invalid. If valid, it checks the skins they have and other account stats, such as wins, battle pass level, account level and more and saves them to a CSV file.

# Preview
![Preview](https://i.imgur.com/US9n4hD.png)

# Results (CSV Preview)
![ResultsPreview](https://i.imgur.com/fVYjgnh.png)

# Features
- Checks for valid / invalid accounts
- Scrapes profile inventory (outfits, pickaxes, gliders and more)
- Scrapes profile data (wins, battle pass purchase and more)
- Supports HTTP proxies
- Saves data for valid accounts in .csv
- Async code
- Cancellation support

# Information
All outfits, gliders, pickaxes and backblings until 5.20.0 have been added.
Proxy feature was not tested as I had no need for it. Use at your own risk.

# Terms and conditions
- This repository is for educational purposes only
- You won't use this application/code to attempt to obtain accounts which are NOT yours (bruteforcing, etc...)
- You won't use this application/code to do anything unlawful or commit crimes
- I am not responsible for any actions done by people who use this code

# Legal
This code is in no way affiliated with, authorized, maintained, sponsored or endorsed by Epic Games or any of its affiliate partners. This is independant and unofficial API. Use it at your own risk.