# CloudFoundry Example Using Rabbit MQ

This example shows the usage of the rabbit MQ backing service. Rabbit MQ provides a flexible queue that can be to publish and subscribe on a channel. There are two variants: The DirectRabbitService which uses the native rabbit lib and establishes the access. The second one is the SpringBasedRabbit, which uses spring dependency injection to have a simplified access to the rabbit service.

## Prepare and Deploy

Go into the manifest and replace the org name d043918trial with your org name.

Create a service instance of rabbit and bind it to the app.

Then build the java war package with Maven
```
mvn clean install
```
Then push to Cloud Foundry
```
cf push
```


