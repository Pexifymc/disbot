This bot list is written in NodeJS. You will need a to [host the site](https://flaviocopes.com/nodejs-hosting) and you'll need a domain so people can access it.

1. Clone the repository into your hosting environment.
2. Edit the `.env` file and fill in all the details. 
    1. To get the Role IDs, [turn on developer mode](https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-). Then go to `Server Settings > Roles` and right click a role and click `Copy ID`.
    2. You'll need a [MongoBD database](https://mongodb.com/atlas).
    3. Create a developer application [here](https://discordapp.com/developers/). You'll need the `Client ID` and `Client Secret`.
    4. You'll also need to create a bot user on the same page and store the `Token`.
    5. Also on the developer application, add your redirect URI under the oauth2 tab. Set it to your domain and then `/api/discord/callback`. For example, `https://botlist.com/api/discord/callback`
3. Install the required dependencies: `npm install`.
4. Run the botlist: `npm start`.
