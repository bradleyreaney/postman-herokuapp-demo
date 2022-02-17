# Postman API automation example 

The following example uses the Heroku restful booker API. Please see [Restful-booker](https://restful-booker.herokuapp.com/apidoc/index.html) for more info.

### How to run the tests
##### Postman collection runner
You can import the collection and environment files into Postman then run the collection there using Postmans collection runner.

[Postman Download](https://www.postman.com/downloads/)
[Using the Collection Runner](https://learning.postman.com/docs/running-collections/intro-to-collection-runs/)

![Postman collection runner](https://assets.postman.com/postman-docs/runner-overview-v8.jpg)

##### Newman CLI
You can also run the collection using the Node package Newman CLI. To do this you'll first need to install Newman using the command `npm install -g newman`

Once thats installed, you'll need to naviagte to the location where the collection and environment files are located and run the following command `newman run <Collection File Name> -e <Environment File Name>`. For our example that would look like this `newman run NimbleHerokuAppDemo.postman_collection.json -e NimbleHerokuAppDemo.postman_environment.json`

![Newman CLI](https://assets.postman.com/postman-docs/newman-running-in-terminal.gif)