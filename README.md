# Hello World Printer
A simple project that has a method for printing out `Hello World`. This project is used to demonstrate dependency management with IBM UrbanCode Build

## Building the Project
### Ant
```
ant dist
```

##### File location
Once built, the `HelloWorldPrinter-dev.jar` file can be found under the `dist` directory

##### Specifying a version
You can optionally pass in the `version` property to specify a version for the build. For example, running
```
ant dist -Dversion=1.0
```
will produce a `HelloWorldPrinter-1.0.jar` file.

### Maven
```
mvn package
```

##### File location
Once built, the `HelloWorldPrinter-1.0-SNAPSHOT.jar` file can be found under the `targets` directory.

##### Specifying a version
You can optionally run `versions:set` with the `newVersion` property to specify a version for the build. For example, running
```
mvn versions:set -DnewVersion=1.0
mvn package
```
will produce a `HelloWorldPrinter-1.0.jar` file.

### Gradle
```
gradle jar
```

##### File location
Once built, the `HelloWorldPrinter-1.0-SNAPSHOT.jar` file can be found under the `build/libs` directory.

##### Specifying a version
You can optionally pass in the `newVersion` property specify a version for the build. For example, running
```
gradle -PnewVersion=1.0 jar
```
will produce a `HelloWorldPrinter-1.0.jar` file.
