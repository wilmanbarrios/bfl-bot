# Fantasy Baseball League Bot

## General Guidelines

1. bot will live in a group chat with all the managers (people that will select players fron de Draft)
2. start Draft by running `/start_round <round_number>`
3. provide the list of players in the round `/players_list <players_list>`
4. a new turn will be given to a group member by doing `/turn <group_member> <time>`
5. bot will send a private msj to `<group_member>` with player list and ask the `<group_member>` to select one player within a set amount of `<time>`
   - to answer `/choose <player_number>`
   - Player that was selected will be send to main group `<group_member> 1`
   - If player don't select a player in the defined `<time>` bot will send `<group_member> ausente`
   - Player can pass a turn and bot will send back `<group_member> paso`
6. when the `round` of seleccion finish, admin needs to close the round `/finish_round`
7. when the round finish the bot needs to collect all answers given by `<group_member>'s` and create a resume list
8. all necesary data will be stored in a file base database for an easy handling
9. bot will be deployed to heroku using free plan
   - [how to deploy](https://github.com/ishan0445/telegraf-telegram-bot-deploy)
   - [tutorial](https://dev.to/ishan0445/deploy-telegram-bot-to-heroku-for-free-telegram-bot-development-part-5-3p29)
   - [heroku pricing](https://www.heroku.com/pricing)
