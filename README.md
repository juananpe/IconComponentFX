# TwitterC
Twitter REST client in JavaFX !

**Table of Contents**

- [Description](#description)
- [Some views](#some-views)
	- [Profile view](#profile-view)
	- [Search view](#search-view)
- [Usage](#usage)
        - [Requirements](#requirements)
- [Build](#build)
- [Modification](#modification)

## Description
This java application provides basic support of Twitter, using the Twitter REST api (through Twitter4j). Among all the functionality, you'll be able to :

- See your profile (tweets, favorites, etc..)
- See anybody profile
- Send tweet
 
The general style of the application is pretty much a visual rip-off of twitter's web interface, using JavaFx. But hey, that's a cool style. The communication with twitter is made with the wonderful [twitter4j](http://twitter4j.org/en/index.html).
 
## Some views
### Profile view
![alt tag](http://i.imgur.com/zO2kxrd.png)

### Search view
![alt tag](http://i.imgur.com/HlsZeBF.png)

## Usage
Just run the provided Jar ! You can download it from the release part of the repo : https://github.com/Vuzi/TwitterC/releases/tag/1.0

You'll need to accept our app to use your twitter account on the first view (either by using the provided link, and copy/pasting the pin code, or by using the framed web view).

Note that the app will save your current access token in a file named 'accessToken.bin' in the current directory. If this file is deleted, modified or moved authentication will be re-asked at the app launch.

### Requirements
- Java 1.8
- A Twitter account

## Build
Note : you'll need an app public/private key from twitter to run this, and replace it in the properties of the pom.xml file :

    <properties>
        <api-key>your-key</api-key>
        <api-secret>your-secret</api-secret>
    </properties>

This a maven project, so all you need to do is what you usually do to build maven project :

    mvn package

And you'll have a runnable jar containing the application and all its dependencies.

## Modification
This project is done with Intellij, so all the related project's files are still here. And yes, the project was commited with API key, but don't worry I've changed them !
