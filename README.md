## 1. How many data your publisher program will send to the message broker in one run? 
> The publisher program will send 5 data messages to the message broker in one run. Each call to publish_event sends one message, and there are 5 such calls in the main() function, each with different user data. <br> <br>
> Example: <br>
`_ = p.publish_event("user_created".to_owned(),
    UserCreatedEventMessage { user_id: "1".to_owned(), user_name: 
    "129500004y-Amir".to_owned() });`

## 2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
> The URL **`amqp://guest:guest@localhost:5672`** being the same in both the publisher and subscriber programs means they are connecting to the same AMQP broker. 

![image](https://github.com/sorfeb/tutorial8-publisher/assets/112263712/221cf6d9-e3f6-49ee-a215-8d7bb969fd9e)

