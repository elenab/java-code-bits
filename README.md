Java Code Samples
=========================

## Apache Camel Examples
###Camel Java Router Project

To build this project use

    mvn install

To compile this project from within Maven, use
```
mvn compile
```
Run:
```
 mvn camel:run
```

### Quarkus example
```
cd quarkus-exampe
```
Run the application in dev mode using: 
```
mvn compile quarkus:dev
```

Then check that the endpoint returns as expected:
```
 curl -w "\n" http://localhost:8080/hello/greeting/Elena  
```
returns:
```
hello Elena
```

Testing:
```
 mvn test
```

Developement mode

`quarkus:dev` runs Quarkus in development mode. This enables hot deployment with background compilation, which means that when you modify your Java files and/or your resource files and refresh your browser, these changes will automatically take effect. 

This will also listen for a debugger on port `5005`. If you want to wait for the debugger to attach before running you can pass `-Dsuspend` on the command line. 

If you don’t want the debugger at all you can use `-Ddebug=false`

.

