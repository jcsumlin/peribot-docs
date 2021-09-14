Peribot's Commands
======

## How to read these documentations

`[prefix][command] [arguments]`

- prefix: your servers chosen prefix (defaults to !)
- command: the command that you are running
- arguments any arguments you need to provide

All commands in the docs will be using the default prefix of "!" if you have changed your prefix just substitute it for every command :)

?> Arguments may be surrounded in [] for separation purposes don't use them in your commands.

### Music Commands

  Peribot's Music cog!

  ?> Peribot will leave an empty voice channel after 60 seconds.

#### !play [song]

   **song**: Either a youtube video URL or the name of a song/video you want Peribot

#### !skip
  
  Skips the currently playing song

#### !queue [page]
  
  Displays the current queue of songs

  **page**: (number) the page in the queue you want to view. Each page is 10 items long.

#### !remove [index]
  
  Removes an item from your queue

  **index**: (number) the number associated with the song you want to remove from your queue.

#### !join
  
  Joins the voice channel you are currently in

#### !leave
  
  Leaves the voice channel and clears the queue


### Setup Commands

#### !prefix [new prefix]

   **new prefix**: the symbol that you want to use as your servers new prefix.

#### !help

  Sends you a link to this site

?> Aliases: !phelp (This helps avoid getting spammed by every bot that may share the same prefix)

#### !ping

Returns the Server latency, API latency, and uptime of the bot
 
Ping ***Pong!***

### Custom commands

Server specific commands that you define! This is great for storing FAQs or important links!

?> Aliases: !cc


#### !customcom add [trigger] [response]

Adds a custom command to your server. This works with images too but only if you set the link to the image as the response to your trigger. Triggers can not overlap with existing commands.

  **trigger**: what the bot is listening for to trigger your response

  **response**: the text Peribot replies with when the trigger is sent
  
?> Exmaple: !cc add hello world | Peribot will listen for !hello and respond with "world"

#### !customcom edit [trigger] [response]

Edits a custom command response to something new.

#### !customcom delete [trigger]

Deletes a custom command from your server

#### !customcom list

Lists all the custom commands on your server.

![custom command list](_media/cclist.png)

### Fun Commands
Fun commands that typically respond with an image or text

#### !cats

Sends a cat gif/image in the current channel
![Cat Gif](https://cdn.nekos.life/meow/0164A.gif)

#### !catsbomb [number]

  **number**: (Optional) the number of images that should be sent

Sends 5 consecutive gifs/images of cute cats!

#### !pugs

Sends a single pug gif/image in the current channel


#### !pugsbomb [number]
  **number**: (Optional) the number of images that should be sent

Sends 5 consecutive gifs/images of cute pugs

#### !eightball [question]

?> Aliases: 8b

  **question**: (Optional) The question that you want Peribot to answer

The bot will answer your question with the typical eight ball fashion.

  **example response**: `Concentrate and ask again.`

#### !topic

Gets a random chat topic to keep the conversation going.

#### !roll [die] [modification] [modifier]

?> Aliases: !r

  **die**: The type of die that you're rolling. Ex: d20 (the d is optional)
  **modification**: (Optional) how to modify the result (Options: + - * /)
  **modifier**: How much to modify your roll by


Rolls a virtual die and returns the result.

**example**: `!roll d20` `!roll d10 + 2` (rolls a d10 die then adds 2 to the result)

#### !flip [user]
  
  **user**: (Optional) The user that you're flipping

Flips a coin ... or a user. But not me.

#### !ded

Shows how dead the chat is... Time to revive it!

#### !uwu [text]
  
  **text**: The text that you want to UwU-ify

This is a very dangerous command, its full potential has not fully been explored. I would recommend extreme caution when using it.


#### !hug [user] [number]

  **user**: The discord user you are trying to hug
  
  **number**: (Optional) The specific hug that you want to send

Sends a random gif of a hug to brighten a users day :)

#### !pat [user] [number]

  **user**: The discord user you are trying to headpat
  
  **number**: (Optional) The specific headpat that you want to send


Sends a random gif of a headpat to brighten a users day :)


#### !kiss [user]

  **user**: The discord user you are trying to kiss

Sends a random gif of a kiss to brighten a users day :)

#### !compliment [user]

  **user**: The discord user you are trying to compliment

Sends a random compliment to brighten a users day :)

![Pinned Message](./_media/compliment.png)

####!bigmoji [emoji]

  **emoji**: the emoji that you want a larger version of

Replies with the a larger image version of the designated emoji.

**example** `!bigmoji :dogoconfused:`

**result** ![](https://cdn.discordapp.com/emojis/674712394341154824.gif)

#### !xkcd [number]

  **number**: (Optional) the specific XKCD comic you want to see. If none is provided it will show you the most recent
  
This command will show you the famous XKCD comics in an embed.

###User Info

####!avatar
Get user's avatar in its full image form.

#### !userinfo [user]

?> Aliases: !ui, !user, !info, !uinfo

**user**: (Optional) The user you want to return information about. Can either be in the form of a mention, their user name, nickname, or user id


Will return some basic information about a given user or yourself
- Their name & discriminator
- User ID
- Nickname
- Status
- In Voice Channel
- Highest Role
- Account Created Date
- Server Join Date

### Server Tools

This will contain server tools and moderation commands that can be used to quickly preform actions on your server.

####bigmoji [emoji]
    
  **emoji**: the emoji that you want a larger version of 

####!serverinfo

?> Aliases: !si, !server, !sinfo

Replies with an embed containing a basic overview of the server in which the command was run

####!rolecolor [role] [color]

  **role**: The role you want to change the color of.

  **color**: The color you want to set the role too. This can be a word or a hex code
     Ex: Red, Green, Orange, #FFF000

  This will change the color of a role. The user must have Manage Roles permissions to use this command. The bot's highest role also must be higher than the role that you are trying to update. Its typically a good idea to have the bot's role at the top of your server's role list. 

  **example** `!rolecolor @Staff Blue`

  **result** Your Staff role is now colored blue!


#### !purge [number]

  **number**: the number of messages that Peribot should delete. Defaults to 5

This will mass delete a set number of messages. The user must have Manage Messages permissions to use this command.

#### !pin [message]

  **message**: The message you want to pin

This will take your message place it in an embed and pin it in the channel that you're in. The user must have Manage Messages permissions to use this command.

![Pinned Message](./_media/pin.png)

#### !kick [user]

Will kick a member. The user must have Kick User permissions

#### !ban [user]

Will ban a member. The user must have Ban User permissions

#### !unban [user]

Will unban a member. The user must have Ban  User permissions

### Moderation Log commands

#### !modlogset channel [channel]

  **channel**: The channel that you want to have logs sent to.
  
This will track all the important things that go on in your server and output all the events to the indicated channel.

#### !modlogset toggle [toggle]

  **toggle**: (Optional) The logging that you want to Enable/Disable. If you dont send a toggle Peribot will send all the toggles and their status.
  ##### Available Toggles
    Join: When a member joins
    Leave: When a member leaves
    Ban: When a member is banned
    Voicechat: When a member is moved in a voice channel
    Message edit: When a message is edited, will show before and after
    Message delete: When a message is deleted, will show message contents
    Role edit: When a role is edited, will show before and after
    Channels: When a channel is created
    Nicknames: When a user's nickname changes
    
Toggles have two states: 

False = not being logged.

True = being logged.
  
#### !modlogset disable

This command toggles the logging system completely. If it is enabled it will disable it and vise versa. 

### Meme commands
A collection of commands use to make and share memes.

#### !bill [text]

  **text** the text to be displayed in between "This is Bill" and "Be like Bill"

  **Example** `!bill He uses Peribot on all his servers`

  **Result**
  ![Bill Loves Peribot](https://images-ext-1.discordapp.net/external/WRf3T_gW36kOzRwJvtWBMhggWl8em-wcP-zRRsv_7jI/%3Ftext%3DThis%2520is%2520Bill%250D%250AHe%2520uses%2520Peribot%2520on%2520all%2520his%2520servers%250D%250ABe%2520Like%2520Bill/https/belikebill.ga/billgen-API.php)


#### !kobayashi [top text], [bottom text]

This will generate a "top text - bottom text" meme using this image

![kobayashi](./_media/kobayashi.jpeg)

You can optionally use just top text or bottom text like this:
`!kobayashi top text only`
`!kobayashi ,bottom text only`

#### !rogu [top text], [bottom text]

This will generate a "top text - bottom text" meme using this image

![rogu](./_media/rogu.jpg)

  **top text**: Text you want to appear at the top of the image. White font color with black outline

  **bottom text**: Text you want to appear at the bottom of the image. White font color with black outline

  Please Note that both the top and bottom text will be fit onto one line and will not wrap based on length. Using longer than normal strings will produce adverse behavior.

You can optionally use just top text or bottom text like this:
`!rogu top text only`
`!rogu ,bottom text only`

### Polls
Create a poll with custom answers!

#### !poll [question], [option 1], [...], [option 10]

  **question**: The question that you want to ask
  
  **option 1-10**: The possible options that a user can choose from, up to 10
  
?> The question and options can be delineated using either a `,` like its shown above or a `|`
  
  Users will be able to react to the poll embed casting their vote for 1 or more option.

#### !quickpoll [question]

  **question**: The question that you want to ask

  This is similar to the !poll command above but instead of custom options it will allow a user to vote using `:thumbsup:` `:person_shrugging:` and `:thumbsdown:` essentially Yes, Maybe, and No. Great for simple questions.
  
  
### Reaction Roles

?> Aliases for all the reaction role commands: !rr [subcommand] [args]

#### !reactionroles list

This will list all the groups of reaction roles that your server has created.

#### !reactionroles role add @[role] [emoji] [group name]

 **role**: The role that users can obtain by reacting to a sent group.
 
 **emoji**: The emoji that users will use to obtain the [role] above.
 
 **group name**: the reaction role group that this role will be added to. To create a group see !reactionroles group add

This will add a role to a pre-existing reaction role group with the provided emoji as the reaction that's to be used to obtain the mentioned.


#### !reactionroles group add [group name]

 **group name**: The name of the group that you want to create
 
 Create a reaction role group that can contain many roles for a user to react to in order to obtain them. This name is case sensitive and you can always see any groups that you've created using !reactionroles list
 

#### !reactionroles send [group name]

  **group name**: the name of the group that you want to send
  
Sends a group of reaction roles for users to obtain by reacting using the preset emojis. Please note that you can only send a specific group once, if you resend this command the previous embed containing reaction roles will no longer work.

When a user adds a reaction to the embed they will be given the associated role and when they remove it it will likewise remove the associated role.
### Reminders

Users can ask to be reminded of things and Peribot will private message them at the prescribed time.

#### !remindme [quantity] [time unit] [reminder]

  **quantity**: the quantity of time units to use when scheduling the reminder
  
  **time unit**: minutes / hours / days / weeks / months. Note: you can use a unit with or without the (s) it doesn't make a difference to the bot.
  
Set a reminder for yourself!

Example: `!remindme 1 hour Do your homework!!`

#### !forgetme

This will remove all your upcoming reminders. This cannot be undone.



### Starboard / Scrapbook

Save all the best moments of your server!

#### !starboard setup [channel] [emoji | :star:] [allowed role | @everyone]

  **channel**: The channel where all your servers best moments will be stored.
  
  **emoji**: (Optional | default :star:) the emoji that the bot will look for on messages to save them
  
  **allowed role** (Optional | default @everyone) The role a user must have to be able to have their messages end up on the starboard
  
?> Aliases: !starboard **set**
  
#### !starboard ignore [channel]

  **channel**: The channel that you want Peribot to ignore for the starboard
  
Peribot will ignore all messages in the given channel when it comes to the starboard. For example your server's log channel, or an admin only channel etc.

#### !starboard emoji [emoji]

  **emoji**: the emoji that the bot will look for on messages to save them

This is command is to make adjustments to a preexisting starboard configuration.


#### !starboard channel [channel]

  **channel**: The channel where all your servers best moments will be stored moving forward.

This is command is to make adjustments to a preexisting starboard configuration.

#### !starboard threshold [integer]

  **integer**: The number of reactions of the configured emoji that are needed for a message to appear on your servers starboard
  
This is command is to make adjustments to a preexisting starboard configuration.

  
#### !starboard add [role]

  **role**: Add a role that's allowed to make it on the starboard
  
This is command is to make adjustments to a preexisting starboard configuration.

#### !starboard remove [role]

  **role**: Remove a role that's allowed to make it on the starboard
  
This is command is to make adjustments to a preexisting starboard configuration.

#### !starboard clear
  
Clears the database of previous starred messages.


### Urban Dictionary

Look up words as they are defined in the Urban Dictionary. Due to the NSFW nature of these definitions this command can only be invoked in a NSFW channel.

#### !urban [search term] [definition number]

  **search term**: The term that you want to search Urban dictionary for.
  
  **definition number**: The definition number you want to see (1-10) 
  
### Welcome Messages

#### !welcome enable [channel] [message]

  **channel**: The channel you want the [message] will be sent in
  
  **message**: The message that will be sent in the [channel] every time a user joins you can add "[user]" to your message and it will be replaced with a mention of the new user.
  
This is a great way to welcome new users to your server and remind them to read rules or something like that!


#### !welcome disable

This will disable the welcome message that you configured above

  