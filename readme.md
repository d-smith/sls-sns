# sls-sns

Simple example of triggering a lambda via sns

Deploy via `sls deploy`

Publsish a message to the topic and observe the result:
```
aws sns publish --topic-arn arn:aws:sns:us-east-1:xxxxx:MyTopic --message Yo
sls logs --function xt1
```

Use `configure-bucket-trigger` to set up s3 notifications that publish to MyTopic
