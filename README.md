# schoolDiary & pzGram
My personal project for an automated School Diary, working with pzGram, my library for the creation of telegram's bot
## pzGram
This is an alpha version, it only supports text messages not other types, and the groups are not supported yet.

Learn more at the wiki on [my site](http://infopz.hopto.org/pzgram)

To create a new bot you need to create a new instance of Bot class:
```python
import pzgram
bot = pzgram.Bot(api_key)
```
After, you can set the list of commands as a dict of command name and command related function:

`bot.set_commands({'/try': try_function})`

At the same way you can set some "timers", functions that are repeated every amount of seconds:

`bot.set_timers({60: send_hello})`

After setting all, you can start the bot writing:
`bot.run()`

## schoolDiary
This program is active on @schoolDiaryBot
This bot is like a real diary and allows you to manage your tests and homeworks easly.
The main featues are:
* Storing your homeworks and tests
* Viewing and Editing your commitments
* Remind your upcoming homeworks and tests
* Save your school time and remind you evening before
* Register your vote and view them by Date, Subject and their average

## Upcoming features
* Integration with ClasseViva API
* Integration with Conofy to add commitments also on my iPhone calendar
* Bring pzGram to a beta version adding the support for all type of message and groups
* Create a wiki for this project on my site
