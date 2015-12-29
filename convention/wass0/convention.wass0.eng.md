Wass0
=========
2015-10-26


Web Assets Standard Structures - 0




This convention describes a way to organize web assets (js and css) in an application.


Why?
------

Using this convention (or any other) might help third party package installers to do their jobs.
 
 
 
So what's the structure?
-----------------------------
 
In this convention, there is a special root directory called "assets" directory, and which contains all the assets
of a given web application.
Typically, the assets directory is the web server root directory itself (often www).

The structure of the assets directory looks like this:

```
- [assets]/
----- js/
----- css/
----- libs/
-------- $libName/
------------ files of the library...
```


So basically, the js and css directories at the root of the assets directory are reserved for the application,
and the libs directory contains automatically installed (assets) packages. 
A package is installed in a $libName directory.
The libName cannot contain forward slash, and therefore forward slashes in the libName should be replaced with a dash.