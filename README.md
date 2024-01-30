<p align= center</p><a href=" " target="_blank"><img src="https://i.imgur.com/cpjB0Ae.png" alt="HazardNuker"></a>


#### GenBot was made by
Love ❌
code ✅

## 🎭・GenBot
> Made this bot for my server to generate account simply by just typing a command like !netflix                             
> It also has a nitro generator, admin command, twitch follow commands, member counter + more other commands like !help and !help [command]

### 🔖・Requirements
* Discord Bot Token | **[Guide](https://discordjs.guide/preparations/setting-up-a-bot-application.html#creating-your-bot)**
* [Node.js](https://nodejs.org/en/) v14.0.0 or newer
* Additionally Twitch tokens and accounts for the commands to work

### 🚀・Getting Started
```
git clone https://github.com/AkramHamd/Gen-Bot_1.0.0.git

cd Account-Generator-Discord-bot
npm i
```

### 📁・Setting up the bot
Go into config.js and put in your discord bot token
and the id's of the channels
```
channels: {
  generator: '',
  nitro: '',
  twitch: ''
},

Token: {
    Discord: 'Your_discord_bot_token',
},
```
after that is done you need to allow intents for the bot to work which is done by going to [discord portal](https://ptb.discord.com/developers/)
enable these 2 options:

 <img alt="intents" src="https://cdn.discordapp.com/attachments/828047793619861557/888421741590884372/Screenshot_2021-09-17_154808.png">

When your done you can do `node index.js` to start the bot.

## 🔰・Features

#### 💾・Customization
In every command at the bottom you can customize the settings for the command accordingly down below
```
module.exports.help = {
  name: "help", //default command 
  aliases: ['help'], //aliases you can use
  category: 'other', //the category the command is in
  description: "List of bot commands.", //description of the command
  cooldown: 7, //cooldown of the command
  usage: '[command_name]', //usage example of command
  example: ["help", "help ping"], //example on how to use command
};
```

#### ❌・Blacklist Users
to blacklist users from the bot completely just add their ID on line 48 in config.js
```
blacklistedUsers: {
  ID: ['ID', 'ID2', 'ID3']//Blacklist any users from the bot by putting their Id's in here
}                        //Just copy the pattern if you want to blacklist more people
```

#### 💻・Generator
In order for the Generator commands to actually work you need to add accounts according to the .txt files in the accounts folder, otherwise it will just say that the service is out of stock
If you want to add more Generator services to GenBot just create a new file named after the new service 
Copy the content of one of the other generator files and just change the names in it

#### 🟣・Twitch
To make Twitch follow fully work you need to go into commands/Twitch/follow.js
At the top change the config to the roles and the amount of followers that they will get
The Raid and spam command are not done yet, feel free to edit those
put the twitch tokens in the tokens.txt file in the Twitch folder

#### 📊・Membercounter
If you want to have membercounter enabled go into events/members/membercount.js and change the guild id and channel id

#### 🧬・Admin
The only Admin command right now is that you can make the bot dm someone a message of choice

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
|🌟Star This Repository If You Liked GenBot!| 
|-------------------------------------------|


