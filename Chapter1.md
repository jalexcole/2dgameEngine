# Setting up the window with LWJGL

## Create the project
1. Create a maven or gradle project
2. Retrieve dependencies from https://www.lwjgl.org/customize and 
copy them into your build.gradle or pom.xml.
    Make sure to use the getting started & native file dialog
3. Set source compatibility to at least 14 preferably the latest of 17 LTS 
4. The net result will be a file structure of:
```
    |-src
    |   |-main\java\io\book
    |       |- App.java
    |   |-test
```
## In the App class
Create a window
```java
package io.book;

public class App {
    Window window = Window.get();
    window.run();
}
```

## Create the Window Class
1. Create a new package jade.
``` java 
package io.book.jade 
```
2. Create a new Java class Window in jade
3. Make window a singleton with an access method of:
```java
public static Window get() {}
```
4. Give the window a width, height, and title field.
5. Create A run function.
6. Implement the LWJGL Getting Started page into the window. 