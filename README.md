# AWS-IoT

### Sending JSOn payload from AWS CLI 
`aws iot-data publish --topic "myTopic" --cli-binary-format raw-in-base64-out --payload "{\"uptime\": 123,\"temp\": 44,\"humidity\": 43}"`

### Sending JSOn payload from AWS CLI  from specified region

aws --region us-east-1 iot-data publish --topic "myTopic" --cli-binary-format raw-in-base64-out --payload "{\"uptime\": 123,\"temp\": 44,\"humidity\": 33}"

### Sending JSOn payload in AWS IoT Core console

Subscribe to some topic say `temp-n-hum`

In Publish to topic section select  `temp-n-hum` and put following in message payload
{
  "uptime": 103,
  "temp": 39,
  "humidity": 45
}


