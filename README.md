# ChampionSuggestionsBot

==== Introduction ====

The Champion Suggestions Bot is a Reddit bot that gives user suggestions on which champions to play for Riot Games' hit moba game, League of Legends. The bot periodically checks reddit comments for its trigger which includes the username (aka Summoner Name) of a player; once the correct trigger fires, the bot will retrieve the player's information using the Riot API, analyze the information and compare it with hundreds of thousands of other players, then make recommendations based on the analysis.

The Champion Suggestions Bot's analytical tool is based on association rules mining. It is similar to, for example, how Amazon.com will give you suggestions on other items to buy when you place an item in your cart. It is designed to give the best suggestions possible while pushing the player to be a little more adventurous.

==== How to Use ====

While logged in on reddit.com, write a comment anywhere in /r/sufficiencybot, /r/leagueoflegends, or /r/summonerschool in the following format:

    championsuggest: <region> <summoner name>

For example:

    championsuggest: na scarra

Wait briefly and you will receive a reply to your comment:

    Champion Suggestions Bot
    -----------------------------
    Hi, you are scarra from NA.
    Your top 3 most played champions in ranked games this season are: Vayne, Diana, Zed
    Recently, you have played: Kog'Maw, Kassadin, Katarina, Thresh, Bard, Zed, Azir, Shyvana, Diana
    -----------------------------
    Based on your personal records in comparison with hundreds of thousands of other players using data mining techniques, I     will make the following suggestions:
    Champions you might want to try: Lucian, Graves, Jinx
    Other champions you might want to try: Yasuo, Kalista, Riven, Lee Sin, LeBlanc, Draven, Nautilus
    -----------------------------
    Champion Suggestions Bot v0.1.1 powered by PRAW, Riot API, and PostgreSQL. Champion Suggestions Bot is not endorsed by Riot Games and does not reflect the views or opinions of Riot Games or anyone officially involved in producing or managing League of Legends. League of Legends and Riot Games are trademarks or registered trademarks of Riot Games, Inc. League of Legends (c) Riot Games, Inc. Click here for a list of commands and change log.

The following URL corresponds to the example above: http://www.reddit.com/r/sufficiencybot/comments/33nl1n/champion_suggestions_bot/cr8cot9

Please do NOT pm the bot, as the bot will not respond to anything. 

==== Common Issues ====

1. I wrote the comment but it didn't respond to me!
A. There are several reasons why this can happen. First, it is likely that you did not write your comment correctly. Your comment must start with "championselect:" or "Championselect:"; no other capitalization patterns/substitutions work. Secondly, you may have misspecified your region and/or Summoner Name.
   If you spot any errors with your trigger, you can either edit your comments very quickly and hope that the bot will rescan your comment, or make a new comment - preferably on /r/sufficiencybot so you do not break any moderation rules. Generally speaking, the bot will ignore comments that are more than 15 minutes old. 

2. The suggestions from this bot are bad!
A. Unfortunately nothing is perfect. While the statistics behind the bot is good, there will always be outliers and you may be out of them.

3. The bot gives few suggestions!
A. The bot will never suggest champions you've played in your last 10 games (excludes ARAMs). Because of this, there are edge cases which you already play the champions the bot is trying to suggest - thus providing you with only 1-2 champion suggestions. 

==== Disclaimer ====

Champion Suggestion Bot is powered by PRAW, Riot API, and PostgreSQL. Champion Suggestions Bot isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing League of Legends. League of Legends and Riot Games are trademarks or registered trademarks of Riot Games, Inc. League of Legends © Riot Games, Inc.
