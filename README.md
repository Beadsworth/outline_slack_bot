# Outline Bot

## Related files

## Setup
Bootstrap Pants (the build tool)
```
./pants goals
```


## Tokens
The slack client currently uses two tokens, both found at:
https://api.slack.com/apps/AB1GJ5QLX/install-on-team


`<app_token>` is `OAuth Access Token`

`<bot_token>` is `Bot User OAuth Access Token`

Tokens should be set as environment variables.

## Run locally in RTM mode
For local runs in Real-Time-Messaging (loop) mode:
```
APP_OAUTH_TOKEN=<app_token> BOT_OAUTH_TOKEN=<bot_token> ./pants run src/python/com/illinoistriangle/bot:bot
```
Local runs are in RTM mode. https://api.slack.com/rtm

## Deployment

Deployment uses the events subscription. https://api.slack.com/events-api

## How to contribute

1. Create a branch
```
git checkout -b <branch_name>
```

2. Make the changes you want

3. Commit your changes

4. Push your branch to github
```
git push origin HEAD
```

5. Make a Pull Request (PR)
Visit the project page https://github.com/TriangleFraternity/outline_slack_bot,
github will ask you if you want to create a pull request for your branch.
