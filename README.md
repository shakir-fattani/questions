# questions
## Java
- What is CompositionAggregation -> in Java, when we create a object and pass any other object in it. plus when you want to update that object you can. because it's a weak relation-ship
- What is Composition -> in Java, When Object is created, and it has other object inside it as final. because it's a strong relation-ship
- Does java support Multi-inheritence? -> Java doesn't support Multi-Inheritence but in Java we have interface, which we can implement and resolve some of our Multi-inheritence problem
- How can we make sure our Single Singleton class is Multi-Thread save? -> we can use `synchronized` keyword or object synchronization with in method `synchronized(object) { }`
- Design Pattern -> 
    1, Singleton Pattern.
    2, Builder Pattern.
    3, Factory Pattern
    4, MVC
    5, Proxy
- When we run `Java -jar file.jar`, how java recognize, which class file to run -> inside jar file, we have `META/MANIFEST` in which we have meta info. and meta attributes name is `Main-Class`

## Android 
- Does android support/Recommend Singleton Pattern -> No, Actually Android doesn't guarantee, that it will not kill you application in background. so after restart Singleton class will be new and it will forget you changes.
- Do we have to do any thing in android to support rotation -> Yes, we have to implement/override onSaveInstance() function for save current application instance, and onCreate function you will get you save data back. and DataFormat is parcelable. so we have to implement Parcelable in our data class

## Spring 
- What is a difference between Spring MVC and SpringBoot -> only major difference is the Server, SpringBoot has Server inside it's package and Spring MVC require you to install Server.
    - Pros for having Server inside
        you don't have to worry about any dependence. and it will run by single command `java -jar spring-boot.jar`
    - Pros for not having Server inside
        you can install, your choice of server(tomcat/jettly/grizly/undertow). plus you can run multiple Spring/J2E applications inside one server.
        in single port. and they can share resources 
