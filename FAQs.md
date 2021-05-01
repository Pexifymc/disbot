I'll add more to these soon. If you have other issues not mentioned here or suggestions, [ask away](https://github.com/Sank6/Discord-Bot-List/issues)

## Why are all bots shown as offline?

To get presence information about other bots, the moderator bot needs to have **presence intents** enabled. ![](https://i.postimg.cc/qRLx062b/image.png)

## How can I host this?

This is an [express](https://expressjs.com/) server like many others, and to host it, you'll need to install and run the file on a VPS (virtual private server) and use a DNS server, to point an A-Name record of your VPS's IP address to your domain. This isn't designed to be hosted on [glitch's](https://glitch.com/) free tier. Read the [setup guide](https://github.com/Sank6/Discord-Bot-List/wiki/Setup-Information) for more information.

## "Invalid OAuth2 redirect URI"

In your Discord [developer settings](https://discord.com/developers) for the application, make sure you only have **one redirect URI** and it is your domain followed by `/api/callback`. Eg, `https://botlist.com/api/callback`.
Also make sure that in your config file, your domain, contains the protocol and does **NOT** end with a `/`. Eg, `https://botlist.com` and not like these: `https://botlist.com/` `botlist.com`

## When will X new feature be added?

I don't actively work on this repository so there is no time estimate for any new feature. However, feel free to make a PR if you have started it and I can review it. Don't open issues asking when something will be added.

## Role issues

 - Check that the Role ID is correct in the config file. 
 - Make sure the role for the Discord bot managing the list has Administrator and it's at the top of the roles list. 