# Samples for Ktor

A collection of ready-to-use samples for [Ktor](http://ktor.io).

* "Hello World" application with various deployment scenarios:
  * [netty](deployment/netty/README.md) &mdash; Netty engine embedded application.
  * [jetty](deployment/jetty/README.md) &mdash; Jetty engine embedded application.
  * jetty-war &mdash; Jetty (war deployment).
  * tomcat-war &mdash; Tomcat (war deployment).
  * [google-appengine-standard](deployment/google-appengine-standard/README.md) &mdash; Google App Engine Standard.

* "Hello World" embedded Netty application with other build systems:
  * maven &mdash; Build with Maven  
  
* Small single-feature samples:
  * async
  * auth
  * custom feature
  * content negotiation
    * gson
    * jackson
  * dependency injection
    * guice
  * locations
  * metrics
  * form post / multipart
  * http2 push
  * static content
  * testable application
  * websocket (tba)
  * sessions (tba)
 
* Big sample applications:
  * [chat](app/chat/README.md) &mdash; Simple chat application using websockets and sessions.
  * httpbin
  * kweet
  * youkube
   
## Running samples

Each sample can be run with 

```
./gradlew :<sample-name>:run
```

Then navigate to [http://localhost:8080/](http://localhost:8080/) to see the sample home page.  
 
Some samples require additional setup as explained in their readme files.
   
## Cut-and-pasting samples

Each sample is a standalone Gradle project that can be cut-and-pasted to get started with your own project. 
Cut-and-paste the directory of the corresponding sample together with 
its build scripts and add [gradle.properties](gradle.properties) from the root
that declares Kotlin, Ktor, and other versions. You may remove reference to the versions that
this particular sample does not use.
