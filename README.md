# A Simple JavaX Server 
The server implements the GET method and uses log4j for logging

## How to use
### Run locally
* Clone the project locally
* Execute: `mvn clean package;java -jar ./target/app_server-0.0.1-SNAPSHOT-shaded.jar;`

The server is set to port `5000`. 

You can access at: `http://localhost:5000/v1/hello`

### Run on Heroku

* If you don't already have a heroku repo, you need to crate one: 
   * `heroku create`
* Push the changes to heroku (the step above would have created a new remote called heroku) 
   * `git push heroku master`
* You are done. You can view the app through heroku using the `heroku open` command and appending the path to the API (`/v1/hello` for example)