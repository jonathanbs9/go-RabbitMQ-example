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



