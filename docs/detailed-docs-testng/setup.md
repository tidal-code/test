---
layout: default
title: Setup
parent: Detailed Docs TestNG
nav_order: 1.1
---


# How to prepare your project

To utilize the Tidal TestNG runner suite you have to add the following dependency to your project. 


```xml
    <dependency>
            <groupId>io.github.tidal-code</groupId>
            <artifactId>wave-testng</artifactId>
            <version>1.0.0</version>
    </dependency>
```

If you are using this artifact, the following artifacts would come along as transitive dependencies

1. Wave
2. Utils

You don't need to download them separately.


## To run tests in IntelliJ Idea

To use the native run button in intelliJ (the little green arrow next to the test name), you need to add a lister to the settings

1. Navigate to Run --> Edit Configurations
2. In the new window, Delete all the existing configurations for the tests by using the '-' button on top
3. Click on Edit Configuration Templates (Link at the left bottom corner)
4. From the list of options click on 'TestNG'
5. Click on Listeners near to the JDK Settings and Parameters
6. Click on '+' and add <b>testngcore.TestListener</b> to the list of Listeners


After completing these steps proceed to the next one - Adding Configuration Directory

### Adding Config Information

In the resources folder, create a new folder named 'META-INF.services'.
In the folder add a file with the name 'io.qameta.allure.listener.TestLifecycleListener'
Then add the following into the file 'testngcore.AllureListener'

NOTE: Once you complete the above steps, quit IntelliJ Idea and start again.