# 🚨 Mondar Group Management Bot 🚨
### Telegram Group Manager Bot + Userbot Written In Python Using Pyrogram.


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Python](http://forthebadge.com/images/badges/made-with-python.svg)](https://python.org)&nbsp;
[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/levina-lab/)


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![LICENSE](https://img.shields.io/github/license/levina-lab/AlexaGroupBot?style=for-the-badge&logo=appveyor)&nbsp;
![Contributors](https://img.shields.io/github/contributors/levina-lab/AlexaGroupBot?style=for-the-badge&logo=appveyor)&nbsp;
![Repository Size](https://img.shields.io/github/repo-size/levina-lab/AlexaGroupBot?style=for-the-badge&logo=appveyor)


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Python Version](https://img.shields.io/badge/python-3.8-green?style=for-the-badge&logo=appveyor)&nbsp;
![Issues](https://img.shields.io/github/issues/levina-lab/AlexaGroupBot?style=for-the-badge&logo=appveyor)&nbsp;
![Forks](https://img.shields.io/github/forks/levina-lab/AlexaGroupBot?style=for-the-badge&logo=appveyor)&nbsp;
![Stars](https://img.shields.io/github/stars/levina-lab/AlexaGroupBot?style=for-the-badge&logo=appveyor)



<img src="https://telegra.ph/file/0a1b9a0331be658e64871.jpg" width="300" align="right">


## Requirements

- Python >= 3.9
- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
- A [Telegram bot token](https://t.me/botfather).
- A [MongoDB URI](https://telegra.ph/How-To-get-Mongodb-URI-04-06)


## Install Locally Or On A VPS

```sh
$ git clone https://github.com/levina-lab/AlexaGroupBot

$ cd WilliamButcherBot

$ pip3 install -U -r requirements.txt

$ cp sample_config.py config.py
```
Edit **config.py** with your own values

# Run Directly
```sh
$ python3 -m wbb
```

# Run On Heroku

## Generating Pyrogram Session For Heroku

```
$ git clone https://github.com/levina-lab/AlexaGroupBot

$ cd WilliamButcherBot

$ pip3 install pyrogram TgCrypto

$ python3 str_gen.py
```

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/levina-lab/AlexaGroupBot/)


# Docker

```sh
$ git clone https://github.com/TheHamkerCat/WilliamButcherBot

$ cd WilliamButcherBot

$ cp sample_config.env config.env
```
Edit **config.env** with your own values

```sh
$ sudo docker build . -t wbb

$ sudo docker run wbb
```

## Write new modules

```py
# Add license text here, get it from below

from wbb import app # This is bot's client
from wbb import app2 # userbot client, import it if module is related to userbot
from pyrogram import filters # pyrogram filters
...


# For /help menu
__MODULE__ = "Module Name"
__HELP__ = "Module help message"


@app.on_message(filters.command("start"))
async def some_function(_, message):
    await message.reply_text("I'm already up!!")

# Many useful functions are in, wbb/utils/, wbb, and wbb/core/
```

And put that file in wbb/modules/, restart and test your bot.

# LICENSE

MIT

```
MIT License

Copyright (c) 2021 TheHamkerCat

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Support 🌺

1. Support Chat : [FAMILYNIRVANA](https://t.me/FAMLIYNIRVANA)
2. Channel Suuport : [FAMLIYNVN](https://t.me/FAMILYNVN)

## Credits 💖

1. [Levina Shavila](github.com/levina-lab)
2. [TheHamkerCat](github.com/thehamkercat)
