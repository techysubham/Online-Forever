# Online-Forever
Make your Discord Account Online 24/7!

----

A Code written in Python that helps you to keep your account 24/7.

</br>

```py
import discord, os, asyncio, datetime, requests

from discord.ext import tasks, commands

client = commands.Bot(
  command_prefix=':',
  self_bot=True
)

async def on_ready():
    client.remove_command('help')
    await client.change_presence(status=discord.Status.online, activity=discord.Game("TESTING"))
client.run(os.getenv("TOKEN"), bot=False)
```

**DO NOT GIVE YOUR TOKEN TO OTHERS!**

Use [uptimerobot.com](https://uptimerobot.com) to make your repl online 24/7.

</br>

> ⭐ Feel free to Star the Repository if this helped you! ;)

----

> Online Forever © 2021 by techysubham is licensed under Attribution 4.0 International 
