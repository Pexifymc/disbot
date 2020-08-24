# About
This is an [open-sourced](https://github.com/Sank6/Discord-Bot-List) Discord Bot List, written in NodeJS, with an [Express JS](https://expressjs.com/) web server and a [discord.js](https://discord.js.org/#/) / [Klasa](https://klasa.js.org/) bot. The bots are stored in a MongoDB database, but no user data is stored or saved. Cookies are used to store discord's oauth data. If you find any issues or bugs, or have a suggestion, feel free to open [an issue](https://github.com/Sank6/Discord-Bot-List/issues).  
Some of the icons used in this website are from [Icons8](https://icons8.com/).


# Setting Up
1. Clone the repo and install the dependencies:
```shell
git clone https://github.com/Sank6/Discord-Bot-List.git
npm i
```

2. Create a config file with the same structure and variables as the example
```shell
cd Discord-Bot-List
```

```shell
Windows:
copy config-example.json config.json

Linux:
cp config-example.json config.json
```

3. Fill in the config file. [(Help)](#config)

4. In your discord application settings, set the callback URL to `/api/callback` and remove all others. Eg, `http://localhost/api/callback`

5. Run the program:
```shell
npm start
```


# Config
 - The domain variable should includes the protocol and **doesn't end with a `/`**. Eg, `http://localhost:8080`.
 - All the roles should be below the role of the bot in charge of the botlist.
 - Most of the variables are Discord IDs. [Enable them in settings](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-).
 - The MongoDB URL can be either a local server or a remote one. [Atlas](https://www.mongodb.com/cloud/atlas) provides a free tier with 500mb.