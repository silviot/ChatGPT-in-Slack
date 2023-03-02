# ChatGPT Bot in Slack

This app demonstrates how to build a Slack app that enables end-users to interact with a ChatGPT bot.
The bot can reply considering the context of a conversation.

## How It Works

You can interact with ChatGPT like you do in the website. In the same thread, the bot remember what you already said.

<img src="https://user-images.githubusercontent.com/19658/222405498-867f5002-c8ba-4dc9-bd86-fddc5192070c.gif" width=500 />

## Run The App

To run this app on your local machine, all you need to do are:

* Create a new Slack app using manifest-dev.yml
* Install the app into your Slack workspace
* Grab your OpenAI API key at https://platform.openai.com/account/api-keys
* Start your app

```bash
# Create an app-level token with connections:write scope
export SLACK_APP_TOKEN=xapp-1-...
# Install the app into your workspace to grab this token
export SLACK_BOT_TOKEN=xoxb-...
# Visit https://platform.openai.com/account/api-keys for this token
export OPENAI_API_KEY=sk-...

python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

## The License

The MIT License
