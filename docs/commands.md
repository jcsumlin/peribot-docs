Peribot's Commands
======

## How to read these documentations

`[prefix][command] [arguments]`

- prefix: your servers chosen prefix (defaults to !)
- command: the command that you are running
- arguments any arguments you need to provide

?> Arguments may be surrounded in [] for separation purposes don't use them in your commands.


### Setup Commands

#### !prefix [new prefix]

   **new prefix**: the symbol that you want to use as your servers new prefix.

#### !help

  Sends you a link to this site

  ?> Aliases: phelp
  
#### !ping

Returns the Server latency, API latency, and uptime of the bot
 
Ping ***Pong!***


### Custom commands

Server specific commands that you define! This is great for storing FAQs or important links!

?> Aliases: cc


#### !customcom add [trigger] [response]

Adds a custom command to your server

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

Sends a single cat gif/image in the current channel
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
  **question**: (Optional) The question that you want Peribot to answer 

The bot will answer your question with the typical eight ball fashion.
  
  **example response**: `Concentrate and ask again.`

?> Aliases: 8b

#### !topic

Gets a random chat topic to keep the chat going.

#### !roll [upperbound]
  **upperbound**: the maximum number of sides on the die you're rolling

Rolls a virtual die and returns the result.

#### !flip [user]
  **user**: (Optional) The user that you're flipping
  
Flips a coin ... or a user. But not me.

#### !ded

Shows how dead the chat is... Time to revive it!

#### !uwu [text]

  **text**: The text that you want to UwU-ify

#### !hug [user]

  **user**: The discord user you are trying to hug

Sends a random gif of a hug to brighten a users day :) 

#### !kiss [user]

  **user**: The discord user you are trying to kiss

Sends a random gif of a kiss to brighten a users day :) 

#### !compliment [user]

  **user**: The discord user you are trying to compliment

Sends a random gif of a compliment to brighten a users day :) 


###User Info

####avatar
Get user's avatar in its full form.


### Server Tools

This will contain server tools and moderation commands that can be used to quickly preform actions on your server.

####bigmoji [emoji]
    
  **emoji**: the emoji that you want a larger version of 

Replys with the a larger image version of the designated emoji.

####serverinfo
Replys with an embed containing a basic overview of the server in which the command was run

?> Aliases: si

####rolecolor [role] [color]

  **role**: The role you want to change the color of.
  
  **color**: The color you want to set the role too. This can be a word or a hex 
     IE: Red, Green, Orange, #FFF000 etc.
  
  This will change the color of a role. The user must have Manage Roles permissions to use this command.
  
####purge [number]
  
  **number**: the number of messages that Peribot should delete.

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

