# Discord Bot for Bilibili

Under developing.

Music bot that plays the audio of Bilibili video and doing local cache. Require python version >= 3.4 and library bs4, discord, youtube_dl and aiohttp.

## Usage

Create `configure.py` with configurations

```
token = 'discord_token'
file_path = 'cache_path'
```

and run in command line

```
python3 main.py
```

## Data Object

### BiliVideoInfo

Store the original url and video information including title, duration, uploader and description

### DiscordPlayer

Base class of players

#### BiliLocalPlayer

Plays the local cache video

#### BiliOnlinePlayer

Plays the online video and doing the local cache

### BiliVideo

Modified from youtube_dl to decode the video address 
