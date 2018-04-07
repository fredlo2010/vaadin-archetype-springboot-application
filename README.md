[![Build Status](https://travis-ci.org/fredlo2010/vaadin-archetype-springboot-application.svg?branch=master)](https://travis-ci.org/fredlo2010/vaadin-archetype-springboot-application)

# Vaadin + Springboot Application Archetype

This is a simple application to create a Vaadin application and Springboot.


1.  Navigate to a folder for the project
2.  Run the command:
    <pre>
    mvn archetype:generate \
        -DinteractiveMode=false \
        -DarchetypeGroupId=com.github.fredlo2010 \
        -DarchetypeArtifactId=vaadin-archetype-springboot-application \
        -DarchetypeVersion=1.0.0 \
        -DgroupId=com.example \
        -DartifactId=pet-store
    </pre>
    
    The project will be created with the following tree.
    
    <pre>
    pet-store
    ├── pom.xml
    └── src
        ├── main
        │   ├── java
        │   │   └── com
        │   │       └── example
        │   │           ├── Application.java
        │   │           └── ApplicationUI.java
        │   └── resources
        │       ├── VAADIN
        │       │   └── themes
        │       │       └── applicationTheme
        │       │           ├── addons.scss
        │       │           ├── applicationTheme.scss
        │       │           ├── favicon.ico
        │       │           └── styles.scss
        │       ├── application.properties
        │       ├── static
        │       └── templates
        └── test
            └── java
                └── com
                    └── example
                        └── ApplicationTests.java
    </pre>

3. Install the application
    <pre>mvn clean install</pre>
    
4. Start the application
   <pre>java -jar pet-store-1.0-SNAPSHOT.jar</pre>
   
   Note: Use your application name in the executable (mine was pet-store) 

5. Visit [http://localhost:8080](http://localhost:8080)

   You should see the message **Welcome to Vaadin + Springboot**

