# Cook Better

Cook Better is a Slack chat bot that recommends recipes based on available ingredients, and user's dietary and health restrictions.

## Demo

![cookbetter-1](https://user-images.githubusercontent.com/18286278/38170174-fd828e36-354b-11e8-8635-256bd4c3bd20.gif)
![cookbetter-2](https://user-images.githubusercontent.com/18286278/38170175-fd923232-354b-11e8-9847-fd213625ac31.gif)

## Slash Commands

### /personalize
<ul>
<li>Use this command to configure any food allergies, dietary restrictions, your health conditions and weight goals.
<li>You only have to do this once and we'll keep your selections in mind whenever you search for recipes!
</ul>

### /searchrecipes
<ul>
<li>Use this command to search for recipes based on the ingredients you have.
<li>You can also search recipes by recipe type, cooking time or find recipes for special occasions.
</ul>

### /surpriseme
<ul>
<li>This command suggests a random recipe every time (while keeping in mind your personalization criteria)!
</ul>

### /cookbetterhelp
<ul>
<li>Come back to this space in case you get stuck and to watch out for any new features we might add!
</ul>

### /recommend
<ul>
<li>This command recommends the recipes based on the recipes you have liked in the past.
</ul>

### /beyourownchef
The command helps the user to create a recipe of their own. It provides some relevant information about the ingredients that the user has provided as the input.

#### This command provides the following information about the input ingredients
<ul>
 <li>The input ingredients that are not ingredients.</li>
 <li>The input ingredients that are not preferred to be used together in a recipe.</li>
 <li>The input ingredients that can be used to produce the best recipe along with the predicted rating of the recipe.</li>
 <li>Additional ingredients that the user should use to create a delicious recipe.</li>
</ul>

## Note
To test the chat bot follow these steps
<ul>
 <li>Create an application on slack using <a href="api.slack.com">Slack API</a>.</li>
 <li>In the application settings add the mentioned slash commands.</li>
 <li>When configuring the slash commands set the Request URL to the URL of the server followed by "/slack".</li>
 <li>Now set up the Request URL in the interactive components to the URL of the server followed by "/slac-interactive".</li>
 <li>Save all the settings.</li>

## Instructions
Follow these instructions to set up the development environment on your local machine.

### Prerequisites
<ul>
 <li>JDK
 <li>IntelliJ IDEA
 <li>Gradle
 <li>Amazon Web Services
 </ul>
 
 ### Development Environment
 
STEP 1: Download and install Java SE Development Kit from <a href="http://www.oracle.com/technetwork/java/javase/downloads/jdk9-downloads-3848520.html">here</a>.

STEP 2: Download and install Intellij IDEA from <a href="https://www.jetbrains.com/idea/download/#section=windows">here</a>.

STEP 3: Download Gradle build tool from <a href="https://gradle.org/releases/">here</a> and follow these <a href="https://gradle.org/install/">instructions</a> for installation.

STEP 4: Clone the repository to your local machine. Open the project in Intellij IDEA. While importing the project, make sure to point to the right Gradle installation folder on your machine.

### Run the Application
To run the application on your local machine, execute the following command in the terminal.

```
gradle build
```

Check out the service.

```
$ curl localhost:8080
```

### Deployment
Execute the following command in the terminal.
```
gradle bootRun
```
The WAR file for the project will be generated in the folder /build/libs.
Deploy the WAR file on Amazon Web Services by following these <a href="https://youtu.be/-ZYQQh8G01A?t=264">instructions</a>.
