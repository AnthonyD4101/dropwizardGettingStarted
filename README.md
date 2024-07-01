# dropwizardGettingStarted

## Learning Objectives

1. Dropwizard Learning (go through ['Dropwizard Getting Started'](https://www.dropwizard.io/en/stable/getting-started.html) guide )
   - Java framework desgined for developing RESTful web services
   - Combines various well-established libraries to provide a complete application
   - Uses things like Jetty, Jersey, Jackson, etc.
   - Getting Started application originally built on Maven, uses `pom.xml` to build
     - Run `java -jar target/getting-started-1.0-SNAPSHOT.jar server hello-world.yml` to run Maven-built helloWorld application
2. Gradle Learning (convert Java project from using Maven's `pom.xml` to Gradle's `build.gradle`)

   - Another build automation tool like Maven, except it uses a Groovy-based DSL, `build.gradle`
   - Functionality is extended through plugins, which can be applied in build script
   - Uses Shadow plugin to create an UBERjar (contains all compiled classes of application, as well as its needed dependencies)

     - Run `./gradlew shadowJar` for Gradle build
     - Run `java -jar build/libs/getting-started-1.0-SNAPSHOT-all.jar server hello-world.yml` to run Gradle-built helloWorld application

3. Docker Learning (deploy project through Docker)
