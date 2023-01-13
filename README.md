# ChatGPT Telegram Bot - @altryne

[![CleanShot 2022-12-02 at 16 08 27](https://user-images.githubusercontent.com/463317/205404516-56ea908e-dd31-4c53-acb7-15f9f6ed379f.gif)](https://twitter.com/altryne/status/1598822052760195072)

This is a Telegram bot that lets you chat with the [chatGPT](https://github.com/openai/gpt-3) language model using your local browser. The bot uses Playwright to run chatGPT in Chromium, and can parse code and text, as well as send messages. It also includes a `/draw` command that allows you to generate pictures using stable diffusion. More features are coming soon.

## Features

- [ ] Chat with chatGPT from your Telegram on the go
- [ ] `/draw` pictures using stable diffusion (version 0.0.2)
- [ ] `/browse` give chatGPT access to Google (version 0.0.3)

## How to Install

### Step 1: Set up your Telegram bot

1. Set up your Telegram bot token and user ID in the `.env` file. See [these instructions](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) for more information on how to do this.

> How to obtain telegram user id? Add telegram [userinfobot](https://t.me/useridinfobot) to your telegram contacts

2. Edit the `.env.example` file, rename it to `.env`, and place your values in the appropriate fields.

### Step 2: Set up your API keys

1. Copy the `.env.example` file and rename the copy to `.env`.
2. To use the `/draw` command, you will need to obtain an API key for stable diffusion. To do this, go to [Dream Studio Beta](https://beta.dreamstudio.ai/membership?tab=home) and sign up for a free membership.
3. SERP_API_KEY is optional. If you want to use the `/browse` command, you will need to obtain an API key for SERP. To do this, go to [SERP API](https://serpapi.com/) and sign up for a free account.

### Step 3: Build the container

1. Open a terminal or command prompt.
2. Navigate to the directory where you installed the ChatGPT Telegram bot.
3. Run `sudo docker build --rm -t <somename>` to start the server. (replace <somename> with anything)

### Step 4: Run the container

1. Run `sudo docker run --restart=always -t -i -d <somename>` (replace <somename> with your chosen name from the step above) 

### Step 5: Chat with your bot in Telegram

1. Open the Telegram app on your device.
2. Find your bot in the list of contacts (you should have already created it with @botfather).
3. Start chatting with your bot.

## Credits

- Me, I just did some minor changes to the bot of @Altryne
- Creator [@Altryne](https://twitter.com/altryne/status/1598902799625961472) on Twitter
- Based on [Daniel Gross's whatsapp gpt](https://github.com/danielgross/whatsapp-gpt) package.
