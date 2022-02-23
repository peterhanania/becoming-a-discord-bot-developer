# Becoming a Discord Bot Developer Guide [Node.js with discord.js]
Hey there, Have you ever wanted to become a JavaScript node.js discord bot developer? Read this guide to get most of my steps and advice when it comes to:
* Learning the basics
* Building your first discord bot
* How to make money online selling bots
* How to publish your own discord bot to the public (making a public bot).
* Coding In General


and much more!


I'm making this tutorial since I found it really hard and confusing at the beginning, and watching others make the same mistakes that I did just made me write this to simplify creating discord bots and getting started into programming.

If you find this useful for you, or for others, feel free to leave a star ⭐ and follow me, it actually means a lot 😊


**THIS PROGRAM WILL TAKE YOU SOME TIME, DON'T RUSH IT, TAKE YOUR TIME OR YOU WILL NOT LEARN ANYTHING.** Before reading make sure you read [My Advice](#my-advice).

> **People always ask me, "How do I create a discord bot? Is it hard??"**
> 
> Well.. It will be hard if you don't know how to start, but once you do, you will be able to create your own discord bot in no time!

Before you start, I'm assuming you know what programming is. If you don't know what it is I please do some research.

### Table of Contents
* [Part 1 - Basic Knowledge](#part-1)
* [Part 2 - Creating your First Discord Bot](#part-2)
* [Part 3 - Publishing Your Discord Bot](#part-3)
* [Part 4 - Making Money Using Discord Bots](#part-4)
* [My Advice in Programming](#my-advice)
* [Recommended Resources](#resources)
* [Contributing](/contributing.md)


### Part 1
In this Part I'll be covering everything from what is Javascript, What is Node.js, What is a database, What is git, How does the discord API work, an introduction to the discord.js Library, and finally Installing your necessary applications to code. I will try to make it as easy as possible to understand. If you are already familiar with this, I advice you skip to [Part 2](#part-2).

<details style="cursor: pointer;">
<summary>Chapter 1: What is Javascript</summary>

#### Chapter 1: What is Javascript?
Javascript is one of the most popular programming languages in the world. It is used to create web applications, games, networking apps. Its constantly growing than any other programming language right now and it is used by top-tech companies like Google, Facebook, Netflix, and Paypal. The average salary for a javascript developer is around 72,000$ per year so its a great opportunity to learn it and to getting a good job out of it.

You can work as a **Frontend Developer** which is responsible for creating the user interface of a website, or a **Backend Developer** which is responsible for the server side of a website, or a **Full Stack Developer** which is responsible for both the frontend and backend of a website.

**Now, what can you actually do with javascript?**
For a long time, javascript was used to create web applications, but now, it is used to create mobile applications, games, networking apps, command line tools and many other things.

**Where does javascript code run?**
Javascript was originally ran on the client side of the browser, which is the browser that is used to view the website. Every website has a javascript engine that can execute javascript code. But in 2009, Ryan Dahl created Node.js, which is a javascript engine that runs on the server side created with c++. Therefore, we can now we can build a backend for our websites, mobile apps, and Discord Bots!

**Resources & Guides:**
* [Source](https://www.youtube.com/watch?v=W6NZfCO5SIk)
* [Guide - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)
* [Guide - W3Schools](https://www.w3schools.com/js/)
* [Guide - Javascript.info](https://javascript.info/)
</details>

<details style="cursor: pointer;" >
<summary>Chapter 2: What is Node.js</summary>

#### Chapter 2: What is Node.js? 
Node.js is an -source, cross-platform JavaScript runtime environment and library used to run web applications outside the client's browser. As mentioned above, Ryan Dahl developed it in 2009. Node.js is used to create server-side web applications and is perfect for data-intensive applications since it uses an asynchronous, event-driven model.

**Getting started with NPM - Node Package Manager (NPM)**
Node.js comes with a package manager called NPM. It is used to install and manage packages. Once you install NPM you'll have a command-line utility to install Node.js packages and dependency management of Node.js packages. Those packages are called modules and they will be used to build your application.

Modules are like JavaScript libraries that can be used in a Node.js application to include a set of functions. To include a module in a Node.js application, use the require() function with the parenthesis containing the name of the module.

For example, if you wanted to make a small website you can use a module called express, you would use the following code:

```js
npm install express
```
which is using the `npm` command line to install the module `express`

with the code:
```js
const express = require('express')
const app = express()

app.get('/', function (req, res) {
  res.send('Hello World')
})

app.listen(3000)
```

In our case, we will be using **discord.js** as a module to create a discord bot.

**Links:**
* [Source](https://www.simplilearn.com/tutorials/nodejs-tutorial)
* [NPM Website](https://www.npmjs.com/)
* [Package Scripts - If Intrested](https://docs.npmjs.com/cli/v8/using-npm/scripts/)
</details>

<details style="cursor: pointer;" >
<summary>Chapter 3: What is a Database?</summary>

#### Chapter 3: What is a Database?
Have you ever wondered where your information is stored? A database is a collection of data that is stored in a structured way. It is used to store data in a structured way so that it can be accessed easily. For example, if you wanted to make a discord levelling bot, you would need to store the users level, xp, id in a database.

Using modules that give us access to databases, we will be storing data and performing operations with that data.
</details>

<details style="cursor: pointer;" >
<summary>Chapter 4: What is git?</summary>

#### Chapter 4: What is git?
Git is a version control system that is used to keep track of changes made to a file and to make sure that the changes are saved.

When creating a discord bot, you will be using git to keep track of changes made to your code.

- You will use to upload your code to the cloud to ensure that you can access the code from anywhere.
- Git will help you recover your old commits if you ever need to.
- You will also use once you want to code a bot with several people.

[Learn Git](https://learngitbranching.js.org)
</details>

<details style="cursor: pointer;" >
<summary>Chapter 5: What is an API & How does the discord API work?</summary>

#### Chapter 5: What is an API & How does the discord API work?
An API (application programming interface) is a set of functions that can be used to perform certain actions. To go into a simpler description, a software that sends information back and forth between a website or app and a user. For example, if you wanted to create a discord bot, you would need to use the discord API function a bot. To simplify for you, did you ever wonder how discord bots work? How do you think bots send messages? They simply send a request to Discord's API that will make the bot send the message.

If you are not familiar with HTTP requests, don't worry. But if you want to learn about them [Click here](https://rapidapi.com/learn/rest-apis/introduction).

Discord's API is based around two core layers, a HTTPS/REST API for general operations, and persistent secure WebSocket based connection for sending and subscribing to real-time events. The most common use case of the Discord API will be providing a service, or access to a platform through the OAuth2 API.

Now you don't have to know much about this, but if you're intrested [Read More](https://discord.com/developers/docs/reference).
</details>

<details style="cursor: pointer;" >
<summary>Chapter 6: Installing your Applications to Code</summary>

#### Chapter 6: Installing your applications to Code
I'm glad you made it till the end of the chapter, but I want to make sure you have everything you need to get started with `discord.js`. I don't expect you to know everything said above. You will learn this with time and research.

**1- Installing Visual Studio Code**
Visual Studio Code is a free and -source code editor for the Microsoft Windows platform. It is used to create and edit code.

[Install it here  - code.visualstudio.com](https://code.visualstudio.com/)

**2- Installing Node.js**
I have mentioned what it is above, now to install it [Click here - nodejs.org](https://nodejs.org/en/). Kindly install version **16.14.0** or higher to run discord.js V13. [Download Link](https://nodejs.org/dist/v16.14.0/node-v16.14.0-x64.msi)

**3- Installing Git (Optional, but Important)**
I have mentioned what it is above, now to install it [Click here - gitforwindows.org](https://gitforwindows.org/), also install [Github Destop - desktop.github.com](https://desktop.github.com/) that will simplify the process of creating a repository on your PC, commiting, etc.
</details>

<br/>

Now that you have a basic understanding everything you need to get started with learning the basics. **Please** Make sure you know the following before going to [Part 2](#part-2);
* Basic Knowledge in Javascript
* Great Understanding of what I Explained above

**How?**
Make sure you check [resources](#resources) for the best resources I recommend you to check out. Make sure you put the time and effort in practicing or else you will be unable to understand the next chapter.

### Part 2
In this Part, I will be teaching you how to create your first discord bot using the `discord.js` module v13; To create a discord bot, Create your test server, setting up your project, making your first discord bot online. Make sure you have all the applications I've mentioned above installed to get started. If you already know this, skip to [Part 3](#part-3).

##### Prerequisites:
Before you begin, Make sure you have a complete understanding of the Javascript Basics. If you are new, Make sure you check out the [Resources](#resources).

If you want to follow the official Discord.js guide, [Click Here](https://discordjs.guide/preparations/).
<details style="Cursor: Pointer">
<summary>Chapter 1: Creating our Discord Bot</summary>

#### Chapter 1: Creating our Discord Bot

To create our bot we need to login to the [official Discord developer portal](https://discord.com/developers/applications). You will then see a "New application" button at the top right like this:
<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/wk2AC8GTdCJnUsG6obvA_newapp.png"></img>
</div>

From there you will be asked to provide a name for your application. You can name yours whatever you want.

You will be redirected to a page with different options for your application. We are wanting to turn our application into an actual Discord bot. To do that we can go to the "Bot" tab on the left:

<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/Q412im2XRH2VyhzjY0lk_discord_bot_tutorial.png"></img>
</div>

Click on the "Add bot" button the right side of your screen. It will create a confirmation popup like this one, simply click on "Yes, do it!"

<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/FckwrDjLQCyZMz7X9WKT_discord_bot_tutorial.png"></img>
</div>

From there you have some important options for your bot. You can change the profile picture, name, and access the bot token.
<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/YypxZp6dTh0ClYCpV4TF_discord_bot_tutorial.png"></img>
</div>

**IMPORTANT:** Your bot's token is basically it's password. Never share your token with anyone. If you believe your token has been compromised click "Regenerate". The bot acts like a user, you give its token, you're giving access to your bot. 

Directly below you will see a checkbox for "Public bot". Make sure to uncheck this if you don't want anyone else inviting your bot to their servers. This is ideal for testing or bots intended for your server only.

[This was taken originally from the Worn Off Keys Blog](https://courses.wornoffkeys.com/blog/how-to-make-a-discord-bot-1#h3skslp7tffhfnsqxmf1gpkwhle7q)
</details>

<details style="Cursor: Pointer">
<summary>Chapter 2: Creating our test Discord server</summary>

#### Chapter 2: Creating our test Discord server

We now need a place to test our bot, it is recommended that you create your own private test server. To do that you can go to the bottom left of the Discord app and click on the plus icon:

<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/RNj0iRq7QrzWwiZTUSdg_discord_bot_tutorial.png"></img>
</div>

You can then click on "Create my own", followed by "For me and my friends", and then give your server a name.

Now that we have our own private Discord server, we can invite our bot to it. Go to the "OAuth2" section of the Discord developer portal:

<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/in2CJdhKT4ev2A0qyf1u_discord_bot_tutorial.png"></img>
</div>

You now want to scroll down to "SCOPES" and select "bot" and "applications.commands". This will make your Discord app into a bot that has access to the new slash commands feature which we will cover in a future tutorial.

Below "SCOPES" you will see "BOT PERMISSIONS" where you can select what permissions your bot will need. When publishing a real bot is it important to only require the necessary permissions. This way server owners don't have to worry about what your bot could do to their server with too many permissions. However while learning we can select the "Administrator" permission to keep things simple. This will give us access to everything we could need.

Once you have selected these three checkboxes your screen should look like this:

<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/ZgRTcnLmQWCjhthkQUlK_discord_bot_tutorial.png"></img>
</div>

At the bottom of the "SCOPES" section you will see a URL with a copy button. This is the link you can give to server owners in order to invite your bot. Simply open this link in a new tab and select your new testing server.

To check if the bot was invited, you can simply go to the server and check if the bot is in the member list.

[This was taken originally from the Worn Off Keys Blog](https://courses.wornoffkeys.com/blog/how-to-make-a-discord-bot-1#h3skslp7tffhfnsqxmf1gpkwhle7q)
</details>

<details style="Cursor: Pointer">
<summary>Chapter 3: Setting up our project</summary>

#### Chapter 3: Setting up our project
We need to setup a new Node.JS project for our bot. First create a new folder in a convenient location and then open Visual Studio Code (VSCode). From there you can drag and drop your folder into your workspace, highlighted here:

<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/6YHBgkfwQhqvVR30P5Ns_vscode.png"></img>
</div>

Press open folder, and select the folder you just created. If you forgot to do so just create one and open it.

VSCode will now show all the files and folders within your newly created workspace folder. Because we just made this folder there are no files listed, but as we add files we will see them here.

To create our project we need to open our terminal. You can do this by clicking "Terminal" then "New Terminal" on the top of VSCode like so:
<div style="padding: 5px 0px;">
<img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/2147490070/images/AmBLaacESWq5VkpnuNxW_vscode.png"></img>
</div>
Or by pressing "CMD | CTRL" + "`" 

This will open a terminal/console near the bottom of your screen. From here we can use different commands to help create our project. If you have never used a console before don't worry, what we need to make our project is fairly simple.

Start by initializing our Node project with:

```node init -y```    

This with initialize our node project. The ```-y``` flag will accept all the default questions it will ask you. If everything worked correctly this should create a "package.json" file in your explorer. Don't worry about what's inside of this file as long as it was created successfully.

We can now install the 3rd party dependencies we need such as `Discord.JS`:

`npm install discord.js dotenv`

**Note:** If you run into permission errors on Windows you may need to run VSCode as an administrator.

Next we need a place to write our own code. At the top left you can click on the new file icon, name the new file `index.js`.

We also need a place to store our bot's token in a secure way. This is why we installed the `dotenv` package earlier. You never want to store passwords, tokens, etc in your source code files. You always want to import those from some external file when possible. This way if you need to share your source code you can simply exclude the file that has your token.

Make a new file called `.env`.
**If you're using Git, you should not commit this file and should ignore it via `.gitignore.`**

Inside you can add in the following text. Be sure to replace "YOUR_TOKEN" with your bot's actual token from the Discord developer portal.

```TOKEN=YOUR_TOKEN```

Now that our project is setup it's time to write the code!

[This was taken originally from the Worn Off Keys Blog](https://courses.wornoffkeys.com/blog/how-to-make-a-discord-bot-1#h3skslp7tffhfnsqxmf1gpkwhle7q)
</details>

<details style="Cursor: Pointer">
<summary>Chapter 4: Writting the Code and Making our First Discord Bot</summary>

#### Chapter 4: Writting the Code and Making our First Discord Bot

Before you start make sure you know what `variables`, `functions`, `conditional statements`, `loops`, and `objects` are. If you have something missing revisit the tutorial and search it up.
 
Once you add your bot to a server, the next step is to start coding and get it online! Paste this code into the file you created earlier, and using the terminal type `node index.js`

```js
// Require the necessary discord.js classes
const { Client, Intents } = require('discord.js');
require('dotenv').config();

// Create a new client instance
const client = new Client({ intents: [Intents.FLAGS.GUILDS] });

// When the client is ready, run this code (only once)
client.once('ready', () => {
	console.log('Ready!');
});

// Login to Discord with your client's token
client.login(process.env.TOKEN);
```

This will Make your first discord bot online, and you should see a message in the console telling you that your bot is online.

After finishing this chapter, its time to practice.

I want you to open the following [Link](https://discordjs.guide/creating-your-bot/creating-commands.html#registering-commands) and start reading and trying to understand how to make a command. Try to read and to paste code and try to make your bot functional. This is a great way to practice and learn. Make sure you take your time. If you have absolutely no idea what you're doing, don't worry, I recommend you start out using a discord bot tutorial [Like this One](https://www.youtube.com/watch?v=JMmUW4d3Noc). Youtube is full of courses, and if you need more help check the coding help servers in [resources](#resources). The main key here is **patience**, don't get frustrated, and don't give up.
</details>


### Part 3
In this Part, I will simplify one of the hardest experiences a discord.js developer experiences when creating & Launching their own discord bot.

##### Prerequisistes:
Before we start, **please** make sure you are familiar with `discord.js`. You've been using it for a while now, and you should be able to get it to work. If not check [How to get Started Properly](#my-advice). 


Let's say you now have been developing small bots for a while (You can know how by reading [How to Sell discord bots](#part-4)) and you want to make a bot that can be used by multiple people. 

You want to make a decent bot for people to use, you want to verify it, you want to add to advertising platforms, you want to grow it etc.. I'm here to help you do all that! To get the most out of it, make sure you read attentively the following chapters.

<details style="cursor: pointer;">
<summary>Chapter 1: Prototyping</summary>

#### Chapter 1: Prototyping

Stop jumping straight into code. Grab a piece of Paper and write down your thoughts on what you want your bot to do, or use Figma, bubble.io. This will help you visualize and organize your thoughts. If you're on a team, start sharing your ideas, write them all down, and follow these steps.

1- **Think ahead**. What do you want your bot to do? What are its features? How is it different from other bots?

2- **Be the User**. If you're the user using your product, would you like the idea?

3- **Discuss & Research**. Take the time to discuss and research more about the categories your bot will offer. Discuss what can go wrong, what can be improved, what can be done better, and what can be done differently.

You can even make a form covering statistical data that you need for your product and send it to your friends who use discord to fill.

Thus, make sure you discuss things like, what database you want to use, what IDE etc. You can read more down.

**Resources:**
* [Find name and domains for bot (brand name)](https://namechk.com)
* [Buy 1$ .xyz domain for 1 year](godaddy.com)
* [Logo Maker](https://looka.com/logo-maker/)

**Keep in mind that your bot should be BETTER than your competitors, if its not it most likely will not grow after release.**
</details>

<details style="cursor: pointer;">
<summary>Chapter 2: Writing the Code & Scaling</summary>

#### Chapter 2: Writing good Code & Scaling

After you've written down your thoughts, you can start writing the code.

The goal here is to make a `fast`, `simple`, and `online` bot. You want your bot to be always fast, you want people to be able to use it without any difficulties (easy to use), and you want to ensure 99% uptime.

If you're with a team make sure you send them this guide, and make sure they understand what you want your bot to do. Also make sure to use GIT or an online IDE ([resources](#resources)) to write down code together.

**1-** **Write Clear Code** (Formatted Code). If you're using visual studio you can use a formatter like [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) or their website https://prettier.io/ to format your code.

**2-** **Pick the right database**. Picking a database depends on the type of data you want to store. If you're going for heavy data go for SQL Databases like MySQL or PostgreSQL. If you're going for light Data and Object based Data go for NoSQL Databases like Firebase and Mongo DB. I personally Suggest you go with Mongo DB. Now after you've picked a database, you need to learn it and write the code to use it.

**3-** **Pick the right IDE**. If you're with a team, make sure they use the same IDE. If you're alone, pick a IDE that you like the most.

**4-** **Writing Fast Code.** How do I write fast code? First Cache Settings that you will require in the `interactionCreate event`. Let's say every time a user requests a slash command, you will need to check if the user is in a guild that has existing data in the database. If you're actually going to request data from the database its gonna be much slower than caching. Caching is basically storing some data in the memory. You can cache with maps, discord collections, or Redis.

As an example;
```js
//ready event
const data = new Map();
global.data = data

client.on('ready', () => {
    client.guilds.cache.forEach(guild => {
        const mongoDBdata = await mongoDB.findOne({ guildID: guild.id });
        data.set(guild.id, mongoDBdata);
    });
});

//interaction event
client.on('interactionCreate', async interaction => {
	if (!interaction.isCommand()) return;

	const { commandName } = interaction;
        const data = global.data.get(interaction.guild.id);

	if (commandName === 'database') {
		await interaction.reply({
            content: JSON.stringify(data)
        });
	} 
});

```

This will slow the load time of the bot, but atleast your commands will be way faster. Therefore make sure you cache.

**- Remove Unnecessary Features**. While writing your code, make sure your feature is actually needed. If you're not going to use a feature, remove it.

**- Avoid Unnecessary Steps**. does your data jump through unnecessary hoops in order to get to the end result?

```js
//example
'incorrect'.split('').slice(2).join('');  // converts to an array
'incorrect'.slice(2);                     // remains a string
```

**- If you're using loops**, Break Out of Loops As Early As Possible. 

**- Avoid High Memory Usage for Cache**. Please use a Customizable Manager Cache depending on the functionalities of your bot to prevent memory leaks. 

As an example;
```js
const client = new Client({
	makeCache: Options.cacheWithLimits({
		MessageManager: 10, // Cache 10 Messages Per Channel.
	}),
});
```

Current Other Options:
```
ApplicationCommandManager: 0, // guild.commands
BaseGuildEmojiManager: 0, // guild.emojis
ChannelManager: 0, // client.channels
GuildChannelManager: 0, // guild.channels
GuildBanManager: 0, // guild.bans
GuildInviteManager: 0, // guild.invites
GuildManager: Infinity, // client.guilds
GuildMemberManager: 0, // guild.members
GuildStickerManager: 0, // guild.stickers
GuildScheduledEventManager: 0, // guild.scheduledEvents
MessageManager: 0, // channel.messages
PermissionOverwriteManager: 0, // channel.permissionOverwrites
PresenceManager: 0, // guild.presences
ReactionManager: 0, // message.reactions
ReactionUserManager: 0, // reaction.users
RoleManager: 0, // guild.roles
StageInstanceManager: 0, // guild.stageInstances
ThreadManager: 0, // channel.threads
ThreadMemberManager: 0, // threadchannel.members
UserManager: 0, // client.users
VoiceStateManager: 0 // guild.voiceStates
```
[Documentation](https://discordjs.guide/additional-info/changes-in-v13.html#customizable-manager-caches)

**5- Scale Propely**. Make sure you scale your bot to the right amount of users. Writing a discord bot designed to scale is a difficult charge. Most developers do the same mistake, if you want to build your own discord bot, please keep in mind that you will have to create several rewrites as the bot grows. With time, if the bot reaches over 25,000 guilds you'll need to get knowledge on sharding, large bot sharding, how ratelimits works etc. You need to start searching for API knowledge and you need to customize the discord.js library as you want. 

[You can read the rest of this Here](https://github.com/shitcorp/Discord-Bots-At-Scale#All-clients)

**6- USE A GOOD HOST!** If you're able to afford buying a host for your bot, please do instead of using platforms like Replit, Glitch, or Heroku. I recommend Google Cloud, AWS, or Digital Ocean. Remember your bot should be fast & online 24/7.

**7- Collect Statistical Data**. Trust me with this,  your bot does not depend on "How Many Servers or Users its in". Those are just numbers. You need make sure you're collecting data like `Joins/Day`, `Leaves/Day`. `Commands Ran/Day`, etc.. You will need monitor this and to know what users are actually liking. You can collect data with services like [Datadog](https://www.datadoghq.com/) or [Statcord - VERY Useful](https://statcord.com/) and simply logging everything into a file, sending it to a webhook, a JSON, a database. Nothing matters, just collect the Data!!

**8- Make it support Rate limiting**. Rate limiting is a feature that Discord has that allows you to limit the amount of requests you can make to the API. Now you don't want people to find ways of abusing the bot so you'll need to develop a good rate limit manager such as command cooldowns, events that cannot be abused. 

**9- Log Properly**. Make sure you are logging when the bot is online, when shard gets connected, disconnected, when a user uses a command, etc. You might need this if your bot is being abused. Don't forget to log all general and command errors to fix them, you can also add a bugreport and feedback command to your bot.

**10- Add a Blacklist System**. Make sure you create an algorythm or manually detect when the bot is being abused, and if it is create a blacklist system that prevents the user or server from using the bot for x amount of time.

To wrap this up, you will have lots of people actually trying to get your bot down. They will try to abuse it, ruin it, don't let that happen. Make sure your database is secured, your bot handles rate limits, abusive behaviour and you're good to go to the next chapter..! 
</details>



<details style="cursor: pointer;">
<summary>Chapter 3: Making the bot Website & Dashboard (Optional)</summary>

#### Chapter 3: Making the bot Website & Dashboard (Optional)

Yay, you're almost done! Now you have a bot that can be used by people. But you want to make it a website, you want people to visit to check its features, its commands, its status, to maybe manage its bot from that dashboard. 

I'm guessing you don't know how to make websites, and you don't know anything about web development and dashboards.

I can't really explain it in here, but I will leave you the steps and resources you should learn before you start.

First you need to learn HTML. This is the language that you use to make your website. HTML is the most basic block of the web. 

To learn it, visit these resources:
* [HTML Tutorial - W3Schools ](https://www.w3schools.com/html/default.asp)
* [CodeCademy HTML Tutorial ](https://www.codecademy.com/learn/learn-html)
* [HTML.com](https://html.com)

Now after you learn the basics, Learn CSS which is the language that you use to style your website. 

To Learn it visit these resources:
* [CSS Tutorial - W3Schools ](https://www.w3schools.com/css/default.asp)
* [CodeCademy CSS Tutorial](https://www.codecademy.com/learn/learn-css)
* [CSS-Tricks.com](https://css-tricks.com)

Now after you're done you'll need to learn javascript to make your website interactive. You already learned it but you just need to learn extra things to make the website interactive.

* [Javascript Tutorial - W3Schools ](https://www.w3schools.com/js/default.asp)

You are free to learn it as you want, there are tons and tons of courses online. This is not easy but remember that great things need time. Trust me you won't regret learning the skill. 

Now you need to start practicing. Start Making Websites! Go to people on discord and offer to make them a free website so that you can get experience from it, or try to make clones of other websites.

Great, you now know how to make a website, how to style it and how to make it interactive. You just created the frontend of your website. Now you need to learn how to make the backend with Node.js using `Express.js`.

Express is a web framework for Node.js. It is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. 

[Watch This Tutorial to Learn Express](https://www.youtube.com/watch?v=SccSCuHhOw0)

Before continuing, Make sure you understand what `Sessions & Cookies` are. 

Now you know how to make the frontend and the backend of the website. Its time to make several test projects to gain more experience before starting your main. 

Similar to the bot the goal here is to make a `fast`, `simple`, and `online` responsive website. You want your website to be always fast, you want people to be able to use it without any difficulties (easy to use), and you want to ensure 99% uptime.

If you're with a team make sure you send them this guide, and make sure they understand what you want your bot to do. Also make sure to use GIT or an online IDE ([resources](#resources)) to write down code together.

You need to create a webpage displaying the problem your solution solves, how your bot works, and benefits for users. Discuss that, then follow the steps below.

**1-** **Write Clear Code** (Formatted Code). If you're using visual studio you can use a formatter like [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) or their website https://prettier.io/ to format your code.

**2-** **Pick the right database**. Picking a database depends on the type of data you want to store. If you're going for heavy data go for SQL Databases like MySQL or PostgreSQL. If you're going for light Data and Object based Data go for NoSQL Databases like Firebase and Mongo DB. I personally Suggest you go with Mongo DB. Now after you've picked a database, you need to learn it and write the code to use it.

**3-** **Pick the right IDE**. If you're with a team, make sure they use the same IDE. If you're alone, pick a IDE that you like the most.

**4-** **Writing Fast Code**
If you're fetching data from a database every time a user requests a page, trust me no one like that. You want to have a fast working website that doesn't take much time to fetch information. Therefore, make sure you cache the data.

Also,
**- Remove Unnecessary Features**. While writing your code, make sure your feature is actually needed. If you're not going to use a feature, remove it.

**- Avoid Unnecessary Steps**. does your data jump through unnecessary hoops in order to get to the end result?

```js
//example
'incorrect'.split('').slice(2).join('');  // converts to an array
'incorrect'.slice(2);                     // remains a string
```

**- If you're using loops**, Break Out of Loops As Early As Possible. 

**5- Collect Statistical Data**. Collect Data to check how many people are viewing your page, what pages are being viewed etc.. You can use Google Analytics or similar tools to collect data. [Google Analytics](https://analytics.google.com/).

**6- Make it support DDOS**. Use Cloudflare as a DNS manager to handle DDOS, and it will create a good free firewall for your website. 

**7- Log Properly**. If you have a login page, monitor the people logging in and out, etc. Also add a limit to people logging in and viewing pages that require user fetching, you don't want to abuse the API. Also, log errors so that you fix them.


Hooray, let's start building the bot dashboard. I will give you the required resources and what you have to do to ensure a great dashboard. You can get started with a simple express and `EJS` dashboard and when you're confident enough you can start going into advanced dashboards using Web Frameworks like `React.js`, `Vue.js`, `Next.js`, or `Angular.js`.

* [Express Discord Dashboard](https://www.youtube.com/watch?v=qujpBixCjIk)
* [React.js Discord Dashboard](https://www.youtube.com/watch?v=_EEcjUVP1DQ)
* [Next.js Discord Dashboard](https://www.youtube.com/watch?v=nYsw2mQ7J6Q)

Follow the intructions given by Anson, listen closely, and as I always say, take your time. Don't rush through tutorials. 
</details>

<details style="cursor: pointer;">
<summary>Chapter 4: Making a support Server</summary>

#### Chapter 4: Making a support Server

Now you have the bot, the website, and what is left is to make a beautiful support server where people can join to get bot support, to test the bot, to chat and more.

You can get started by picking a server style from the list below.
* [discord.style](https://www.discord.style/)
* [discordtemplates.me](https://discordtemplates.me/)

Then set up the roles, permissions, add what you want like a verification system, welcome message, etc. You can join other bot servers to have a glimpse of what you want to add.

Now make sure you make a working ticket system, hire moderators and support members to help members out.
</details>

<details style="cursor: pointer;" >
<summary>Chapter 5: Testing Before Release</summary>

#### Chapter 5: Testing Before Release

Okay, everything is done. But how will my bot and website perform publicly? Before releasing the bot, re-test every feature twice then get people you know to test it with you, to invite your test bot to some small extra servers and you should expect tons of bugs here, make sure you fix them all.
</details>


<details style="cursor: pointer;">
<summary>Chapter 6: Releasing the Bot</summary>

#### Chapter 6: Releasing the Bot

I'm so proud of you! You've made a bot, a website, and a support server. Your bot is now fully functional and its time to release it. Once you release, your bot will most likely grow VERY Slowly, I mean 1-2 servers a day, or sometimes weeks. Don't worry, success comes with time. All big bots on discord took years of work even mine.

Therefore, I followed this chapter up with Advertising Tips to help you grow the bot.
</details>

<details style="cursor: pointer;">
<summary>Chapter 7: Adverting and Growing the Bot</summary>

#### Chapter 7: Adverting and Growing the Bot

My Bot is growing really slowly, its barely being used.. what do I do!? Here are some of my few tips into growing your bot. Now if your bot has bigger competitors with similar features, I'm sorry but I'm afraid it will take more effort to grow. 

**1- Advertise your bot.** Advertise your bot on platforms like:
* [Top.gg](https://top.gg)
* [Discord.me](https://discord.me/)
* [Discordbotlist.com](https://discordbotlist.com/)
* [Disforge.com](https://disforge.com/)
* [Discordlabs.org](https://discordlabs.org/)

**2- Create Vote Reward.** Reward users that vote for your bot so that It gets more votes.

**3- Open source your bot.** By doing this you will allow thousands of people to steal your work but it will bring you some attention. If your bot has tons of features and you feel like people will easily discover it, open source it and tell people to check it out in coding servers. [resources](#resources)

**4- Top.gg Auctions.** If you are able to pay, [Visit this](https://top.gg/advertise)

**5- Create Tutorials.** Create some videos about some outstanding features of your bot and post them to social media platforms.

**6- Add your bot website to your status and join coding servers and just be active.** Trust me this works well.

</details>

<details style="cursor: pointer;">
<summary>Chapter 8: Receiving Funds</summary>

#### Chapter 8: Receiving Funds

Hosting isn't cheap, buying a domain isn't cheap, therefore you need to make sure you have a premium plan for your bot. Make something intresting that people will love at a good price. You can use platforms like Patreon or PayPal to receive money /or donations. Take your time in this, your bot is already out you have some time to migrate some top commands used by people to premium features.
</details>

<details style="cursor: pointer;">
<summary>Chapter 9: Discord Verification</summary>

#### Chapter 9: Discord Verification

Once your bot hits 75 unique servers, you will have the ability to verify your bot. This will allow you to gain more people to invite your bot to. If you do not verify, people won't be able to invite your bot to any more than a 100 servers. By unique I mean, your bot needs to be in normal servers not bot spam & Testing servers. Try and get your bot invited to normal servers and kick the bot from servers that are spam. 

#### Verification Information

- If you are in a team, the owner gets verified, which verifies the whole team. [Source](https://blog.discordapp.com/the-future-of-bots-on-discord-4e6e050ab52e)
- If you can't provide ID verification, you could transfer ownership of your team to another member so they can do the verification process. [Source](https://discordapp.com/channels/613425648685547541/696891424041598978/697495117069680711)
- The Stripe verification piece is on the user itself, but the other parts of the form are per-bot.
- You do NOT need a Stripe account to verify, only your ID. [Source](https://discordapp.com/channels/613425648685547541/697236247739105340/697248540275114044)
- Verification is only needed if you are in more than a 100 servers, however you can start early at 75+ servers. [Source](https://blog.discordapp.com/the-future-of-bots-on-discord-4e6e050ab52e)
- Will verification be available for bots in less than 75 servers? Currently, no. We may raise or lower the limit in the future. [Source](https://discordapp.com/channels/613425648685547541/697236247739105340/697487149133725777)
- Verification time should be about a five business day turnaround. [Source](https://discordapp.com/channels/613425648685547541/697236247739105340/697492876875137116)
- Verification seems open to everybody as long as they are in the age of using Discord, which is 13.
- Verification is done by a human, no need to worry about bots misundestanding you.

####  What are Privileged Intents? [Source](https://discordapp.com/developers/docs/topics/gateway#privileged-intents)

`GUILD_MEMBERS` lets you catch events when people update themselves or join/leave a server.
`GUILD_PRESENCES` lets you catch status updates such as online, idle & games/custom statuses.

NEW:
`GUILD_MESSAGES` lets you access message.content sent to a server.
```
GUILD_MEMBERS (1 << 1)
  - GUILD_MEMBER_ADD
  - GUILD_MEMBER_UPDATE
  - GUILD_MEMBER_REMOVE

GUILD_PRESENCES (1 << 8)
  - PRESENCE_UPDATE
```

####  Non-exhaustive list of accepted IDs [Source](https://stripe.com/docs/connect/identity-verification-api#acceptable-id-types)

- Passport
- Driver license (front/back)
- ID card (front/back)
- Resident permit ID/U.S. Green Card/North Carolina Resident ID
- Border Crossing Card
- Child ID card
- NYC Card
- U.S. visa card

It depends from country to country, but in general, you'll want a valid, government-issued photo id. This can be a driver's license, passport, federal ID, or something else in that category. The specifics to where you are located may be different. If you are required to get verified, Stripe will let you know during the process if your ID is OK or not. For a list for countries other than the US, see here: https://stripe.com/docs/connect/identity-verification-api#acceptable-id-types. However, **this is NOT EXHAUSTIVE OF ALL THE COUNTRIES THEY SUPPORT.**

If you don't have an ID, contact support, they'll help. Also apparently, in the U.S. you can get a state ID with parental conscent.

#### Other stuff

- Stripe is already a trusted platform for payments, no need to worry about your data there. They don't make money off your data, they make money off of transaction fees.
For those worrying about data being stored in a U.S. server, I get that, but we don't really have any other choice sadly. I'm not saying that's how it should be, I'm saying that's how it is.
- Can our bots have verified support servers?
It's been asked a couple times. On a note for me to think about, but nothing right now. [Source](https://discordapp.com/channels/613425648685547541/696891424041598978/697254807429447720)

### Questions about the verification form

####  WHAT SYSTEMS AND INFRASTRUCTURE DO YOU USE?

How do you run your bot?
 - OS with version, if possible.
 - Libraries (including version) and programming language.
 - Databases, if any.
 - Hosting solution. E.g. List your provider or self-hosted.

####  HAVE YOU SECURED ACCESS TO YOUR SYSTEMS AND INFRASTRUCTURE?

Is your server secure? Can anybody access that data? 

####  DOES YOUR APPLICATION UTILIZE OTHER THIRD-PARTY AUTH SERVICES OR CONNECTIONS? IF SO, WHICH, AND WHY?

The third party services are more like "Does your bot also do Twitch OAuth so you can connect Discord to Twitch?" [Source](https://discordapp.com/channels/613425648685547541/696891424041598978/697490654665768960)

####  All the stuff about storing data

If you do not store any data, just write `I don't store data.` If you store data about e.g. levels and currencies, you should write that. Since data is anonymized, it's most probably fine. Anyways, lying would get you in even more trouble. When in doubt include it.

From what I understand, end user data is data generated by users (like their username, message content, etc). Snowflakes aren't because they are generated by Discord.

##### Does storing data count if it's logging to a text channel?
No, it's literally just sending Discord's data back to Discord. It's fine.

###  WHY DOES DISCORD GET ACCESS TO MY ID?
Probably because they need to verify that Stripe is not lying to them about the verification. They specifically said that they don't keep any data.

If you need me to help with verification, ask me in my own [Bot's support server](https://pogy.xyz/support).

[Taken Officially from Here](https://gist.github.com/jakobbouchard/647404a48c7df34aeb21dce2c511b4a0)
</details>

<br/>

Great job, you now have your own discord bot. I hope you enjoyed this Part. If you have any questions or advice, feel free to ask me in my own [Bot's support server](https://pogy.xyz/support).


### Part 4
I'm sure we all thought about this, I want to make money. But how do I make money? Most of the people try to make money stealing other people's work and that's totally not okay. Money doesn't grow on trees, you want money you need to work. You don't want to work, well that's not an option when it comes to money. 

**1- Get the experience you need.** Practice making all types of discord bots. Go to discord, join the suggested discord servers in [resources](#resources) and offer to make **free** bots for people. Now those bots will give you great experience and that's what you're looking for. You need to learn how to communicate properly with a client. Address your client formally, and make sure you understand what they are asking for. 

**2- Post all of those on your github profile and Portofolio and Work on a good Profile.** This will attract lots of people to your github profile, some of those people will be your clients. If you're really good at what you're doing and you have a good portfolio, you will get more clients. If your projects are not well made, you will get less clients. Your goal here is to have a good looking github profile and a good looking discord profile.

**3- Be active in coding servers.** Not only this will help you communicate with others, it will help you learn more so that you'll be able to make any sort of discord bot your client is asking for. Everytime a user asks for help, help them in channel or DMs, trust me it will give you lots of fame and experience.

In my opinion, that's all you need. Make sure you have a good portfolio, a good github profile, and a good discord profile. Make sure your projects are outstanding so that they receive traffic from people. Now open your dms, and start talking to clients. (Add your discord tag to your profile or make a discord server where you sell bots there) 

This will help you find a job in the future, and make money 😉

Good luck!! If you have questions or advice, feel free to ask me in my own [Bot's support server](https://pogy.xyz/support).

### My Advice
I have been developing websites and bots for a long time now, and here is what I can advice you.

**1- Its not about memorizing, its about understanding.** If you understand the concepts you can always come up with a solution. Be a problem solver, **let google be your resource**.

**2- Coding is basically like Playing Lego.** As you keep learning you will get more pieces to build with. The more the pieces you have, the more complicated things you can build.

**3- If you want to get better at coding, Find a mentor.** Learning on your own is really hard, you'll never know if you're doing things correctly. A mentor will provide guidance and will correct you.

**4- Stop jumping straight into code.** Get a paper and write down what you visualize.

**5- Age doesn't matter. What matters is if you enjoy it or not.** Don't waste your time on something you do not enjoy. You can try it out, you might end up liking it. You don't need to be an expert at math, nor have a degree. Stay true to yourself and find discord communities that will motivate you and guide you. [resources](#resources).


**6- Don't loose yourself in Tutorial Hell.** Learn the basics and jump into projects.

### Resources
I advice you to check out these resources.

**1- Youtube Channels**
* [Worn Off Keys](https://www.youtube.com/channel/UChPrh75CmPP9Ig6jISPnfNA). Great for discord tutorials.
* [Anson The Developer](https://www.youtube.com/channel/UCvjXo25nY-WMCTEXZZb0xsw). Great Dashboard Tutorials.
* [Travery Media](https://www.youtube.com/c/TraversyMedia). Great General Coding Tutorials.

**2- Discord Coding Servers**
* [Worn Off Keys](https://discord.gg/wornoffkeys). Once of the best discord servers to ask for discord help. Very welcoming community.
* [Discord.js](https://discord.gg/djs). The official `discord.js` server to help you solve errors and get general help.
* [The Coding Den](https://discord.gg/code) & [The Programmer's Hangout](https://discord.gg/programming). Great places to chat and meet developers.
* [Discord Developers](https://discord.gg/discord-developers). Receive discord API Updates.
  
**3- Hosting Providers**
* [DigitalOcean](https://www.digitalocean.com/)
* [AWS](https://aws.amazon.com/)
* [Vultr](https://www.vultr.com/)
* [GitHub education](https://education.github.com) Free credit and other offers for students.
* [Google Cloud](https://cloud.google.com/) free tier

**4- Online IDEs**
* [Replit](https://replit.com/)
* [Glitch](https://glitch.com/)
* [JSBin](https://jsbin.com/)
* [CodePen](https://codepen.io/)
  
**If you want me to add a certain resource, email me at `peter@pogy.xyz`.**

Finally, If you liked this repository, feel free to leave a star ⭐ and follow me, it actually means a lot.


