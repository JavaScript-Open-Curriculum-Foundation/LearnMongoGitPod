# MongoLearnPod
An education GitPod module intended to teach individuals how to use mongo on any machine.

A possible unit as of the 

Here we are applying the idea of [GhostPlate](https://github.com/HansUXdev/GhostPlate) built on GitPod to education instead of Industry at scale ...

# Read and Code Along!
Assuming you are logged into github, then just click the button below. Phone, Tablet, Mac, Windows, Linux, Chromebook, as long as GitPod runs, you can learn how to code, anywhere!

<p align="center">  
   <a href="https://gitpod.io/#https://github.com/HansUXdev/MongoLearnPodt"><img src="http://gitpod.io/button/open-in-gitpod.svg" alt="Open on GitPod" height="50px"/></a>  
</p>

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
1. Use GitPod to startup a mongoDB environment.
2. Use docker exec to access the mongoDB Shell 
3. Distinguish between the name of a docker image (mongo) and the container name (learn-mongo)
4. Use NPM Scripts to store docker commands such as docker exec for mongo shell

# About me
Hans McMurdy is an experianced web developer and coding teacher.

## About
This is a brief mongo tutorial in GitPod and originally built for docker and docker compose which you can see [here](https://github.com/HansUXdev/OSS-Books/tree/master/JavaScript-First/00-JavaScript-DataBases/mongo).

## Using Mongo Shell to build a database
  Type the following into a NEW terminal: ` mongo`. Because no one in chat wanted to help me run it in headless mode (thanks, support :-) ).
  
  Lets go ahead and create a new *collection* and use it. 

  Type the following into the terminal: `use mongo`. 

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

# Conclusion


## Key learnings

## Tips and advice

   
1. [w3-Resource](https://www.w3resource.com/mongodb/databases-documents-collections.php#:~:text=A%20collection%20is%20analogous%20to,are%20not%20same%20in%20structure.&text=In%20a%20relational%20database%20like,formula%20defining%20structure%20of%20data)
   
2. Try the [freecodecamp lesson](https://www.freecodecamp.org/news/learn-mongodb-a4ce205e7739/)



## Final thoughts and next steps
   
1. Try this out with the local docker version.


## Open Source Book Candidate
This a standalone educational module unit. If you like it and want to see more on this topic, give it a stars. If there is enough interest in it, I'll add it too [JavaScript-First](https://github.com/HansUXdev/JavaScript-First) is an open source book that teaches people how to code with JavaScript using the node.js runtime environment rather than a browser and by the end, you will build a server and a website using JavaScript.

<p align="center">
   <a href="https://github.com/HansUXdev/JavaScript-First">
      <img src="https://raw.githubusercontent.com/HansUXdev/JavaScript-First/2acf5840c15af96602aceb66303ea69c5b75e344/logo.svg" style="max-width:50%;" height="200px" alt="JavaScript Logo"/>
   </a>
</p>
