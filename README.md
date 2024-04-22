## 1. How many data your publisher program will send to the message broker in one run? 
> The publisher program will send 5 data messages to the message broker in one run. Each call to publish_event sends one message, and there are 5 such calls in the main() function, each with different user data. <br> <br>
> Example: <br>
`_ = p.publish_event("user_created".to_owned(),
    UserCreatedEventMessage { user_id: "1".to_owned(), user_name: 
    "129500004y-Amir".to_owned() });`

## 2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?