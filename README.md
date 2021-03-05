# go-RabbitMQ-example

![image](https://user-images.githubusercontent.com/32901911/110122792-cea29b80-7d9e-11eb-835e-5ab05195fee2.png)

## Why use message broker?
- Helps developers to implement more resilent distributed systems that are able to handle parts of the application going down.
- We can effectively decouple both our back-end and front-end applications 

## Advantages:

![image](https://user-images.githubusercontent.com/32901911/110123294-8041cc80-7d9f-11eb-83f3-f5f4f725df84.png)



### Steps
1- Instance of rabbitMQ with docker

docker run -d --hostname my-rabbit --name some-rabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management

2- Enter RabbitMQ.  In web browser: 

localhost:15672
username: guest
password: guest

![image](https://user-images.githubusercontent.com/32901911/110125101-b6804b80-7da1-11eb-804b-7be418982ec2.png)


## Test messages

* Publish message
> go  run main.go

![image](https://user-images.githubusercontent.com/32901911/110133704-5e4e4700-7dab-11eb-985a-01a81497af34.png)


* Consume message
> go run consumer.go
 
![image](https://user-images.githubusercontent.com/32901911/110133780-7920bb80-7dab-11eb-8e8a-78f820a9be01.png)


Every time we want to publish a message, you have to run main.go. 
If Consumer is listening, will hear the messages, and print them. If there are no messages on queue, will display  [*] Esperando por mensajes ... 
