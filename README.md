# backlog2slack
Post Backlog update message to Slack.

thx. https://qiita.com/kosuge/items/051922673cf57203f8db


## requirements
* Serverless Framework.

## deploy
1. Make CustomIntegration on your Slack and get Incoming Webhook URL.(like: `https://hooks.slack.com/services/XXXXXXXX/YYYYYYYY/zzzzzzzz`)
2. Make `config.yml` from `config.yml.sample`.
3. Run following script.
  ```
  $ npm run deploy
  ```
4. Set Webhook URL to Backlog.
  ```
  https://xxxxxxxx.execute-api.us-east-1.amazonaws.com/dev/b2s/yyyy

  xxxxxxxx: APIGW endpoint
  yyyy: Slack room name
  ```


## remove
1. Run following script.
  ```
  $ npm run remove
  ```
