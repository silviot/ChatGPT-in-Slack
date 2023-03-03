# ChatGPT in Slack

Introducing a transformative app for Slack users, specifically designed to enhance your communication with [ChatGPT](https://openai.com/blog/chatgpt)!
With this app, you can seamlessly interact with ChatGPT through Slack channels, streamlining your planning and writing processes with the power of AI.

Please check [the product website](https://seratch.notion.site/ChatGPT-in-Slack-749f2041a62a4c00ad9b964d952034b4) for more details!

## How It Works

You can interact with ChatGPT like you do in the website. In the same thread, the bot remember what you already said.

<img src="https://user-images.githubusercontent.com/19658/222405498-867f5002-c8ba-4dc9-bd86-fddc5192070c.gif" width=500 />

Consider this realistic scenario: ask the bot to generate a business email for communication with your manager.

<img width="500" src="https://user-images.githubusercontent.com/19658/222609940-eb581361-eeea-441a-a300-96ecdbc23d0b.png">

With ChatGPT, you don't need to ask a perfectly formulated question at first. Adjusting the details after receiving the bot's initial response is a great approach.

<img width="977" src="https://user-images.githubusercontent.com/19658/222609947-b99ace0d-4c90-4265-940d-3fc373429b80.png">

Doesn't that sound cool? 😎

## Running the App on Your Local Machine

To run this app on your local machine, you only need to follow these simple steps:

* Create a new Slack app using the manifest-dev.yml file
* Install the app into your Slack workspace
* Retrieve your OpenAI API key at https://platform.openai.com/account/api-keys
* Start the app

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
