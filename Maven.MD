# Maven


- Maven is a project management tool.

- Most popular use of maven is for build management and dependencies.
  
-  When building a Java project we may need additional JAR files. One approach is to download the JAR files and manually add to our class-path. We tell the maven the projects we are working with. Maven will go out and download the JAR files for those projects for us. And maven will make those JAR files available during the compile/run.

	![maven img](https://github.com/sovisrushain/Notes/blob/main/data/mvn01.png?raw=true)

    1. Read Config file
    2. Check local Repo
    3. Get from remote Repo
    4. Save in the local Repo
    5. Build and Run

- When maven retrieves a project dependency it will also download the supporting dependencies. 

- When we build and run the app based on the config file, maven will add JAR files accordingly. 

- Also maven provides a standard directory structure. 

- For new developers joining the project, they can easily find the code, properties files and unit tests etc.:

## Advantages of Maven

1. Dependency management.
2. Building and running our projects.
3. Standard directory structure.


## POM file

- **P**roject **O**bject **M**odel file : POM file

- This is a configuration file for projects.

- Located in the root of our maven project.

## Repository Types

1.Local Repository
    
    Located on developer’s computer

    Our local cache

    Maven will search this repository first before going in to the maven central repository

    `Unix/Mac OS X – ~/.m2`

    `Windows – C:\Documents and Settings\{your-username}\.m2`
2.Central Repository
        
    By default maven will search maven’s central repository(remote)

    Requires an internet connection

    Once files are downloaded, they are stored in local repository

    [`https://repo.maven.apache.org/maven2/`](https://repo.maven.apache.org/maven2/)


