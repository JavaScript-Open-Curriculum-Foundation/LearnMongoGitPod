# MongoLearnPod
An education GitPod module intended to teach individuals how to use mongo on any machine.
Here we are applying the idea of [GhostPlate](https://github.com/HansUXdev/GhostPlate) built on GitPod to education instead of Industry at scale ...

# How to use?:
See that button?
Click it with your right index finger and wait.
If you use any other finger I will bite it off.
[![Open in Gitpod](http://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io#https://github.com/gitpod-io/gitpod-status)


Then follow the directions inside the GitPod. Don't worry its still better than Microsoft documentation...

## Unit Learning Objective
Students should be to:
1. Use Docker Compose to start and stop mongoDB environment
2. Use Docker, Terminal & MongoExpress to teach basic mongoDB concepts
3. Distinguish between the name of a docker image (mongo) and the container name (learn-mongo)
4. Use NPM Scripts to store docker commands


# What did you build
Today we'll be learning how to use Docker Compose to learn MongoDB.

## Unit Learning Objective
Students should be to:
1. Use Docker Compose to start and stop mongoDB environment
2. Use docker exec to access the mongoDB Shell 
3. Distinguish between the name of a docker image (mongo) and the container name (learn-mongo)
4. Use NPM Scripts to store docker commands such as docker exec for mongo shell

# About me
Hans McMurdy is an experianced web developer and coding teacher.

## About
This is a brief mongo tutorial in GitPod and originally built for docker and docker compose which you can see [here](https://github.com/HansUXdev/OSS-Books/tree/master/JavaScript-First/00-JavaScript-DataBases/mongo).

## Using Mongo Shell to build a database
  Lets go ahead and create a new *collection* and use it. 

  Type the following into the terminal: `use learnMongo`. 

  We can then show the database we are using by using the `db` command.

  Next we are going to insert some data into our new database.
  To do this we'll use the the [insert](https://docs.mongodb.com/manual/tutorial/insert-documents/) command.


  ```js
  db.info.insert(
    {
      "country": "United States of America", 
      "state": "Arizona", 
      "cities": ["Phoenix", "Mesa", "Chandler"]
    }
  )
  ```
  This will insert a new *document* into the info *collection*.

  **Exercise**
  Next, you should come up with 2 other states, with atleast two cities in each.

  Finally, we will use the [.find()]() method to find the document with a state of Arizona.

  ```js
  db.info.find({state:'Arizona'}).pretty()
  ```
  Note that the [.pretty()]() command just formates the data more properly.


  By the end of the exercise your terminal should look something like following but with different examples:
  [![](exercise1.png)]()

  If we open mongo-express, we should see a new database appeared. We can also use the terminal command `show dbs` to display them in terminal.

  [![](mongo-express02.png)]()
  [![](mongo-express03.png)]()
  [![](mongo-express04.png)]()


## Using NPM Scripts
  # Package.json is used to demostrate NPM Scripts for use with docker
  Students should be able to:
  * Identify the package.json file and the script section
  * Modify the package.json file to add the docker command
  ```
  "mongo": "docker exec -it learn-mongo mongo",
  ```
  * Distinguish between the name of the docker image (mongo) and the container name (learn-mongo)

  * Demonstrate Mongo Terminal Commands
  1. Running with docker compose
      - ```docker exec -it learn-mongo mongo```

# Conclusion
## Key learnings
## Tips and advice
## Final thoughts and next steps
