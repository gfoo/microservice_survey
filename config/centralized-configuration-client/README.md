Test client :

`http://localhost:8080/message`

Should return `message` commited in this config file : `https://github.com/gfoo/microservice_survey/blob/main/config/a-bootiful-client.properties`


Commit new config message, reload configs with the actuator by launching a POST:

`curl localhost:8080/actuator/refresh -d {} -H "Content-Type: application/json"`

Relaunch the above endpoint `message` and chack that the new commited message is provided.

