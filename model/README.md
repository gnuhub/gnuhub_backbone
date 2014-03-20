model & collection
==========================

[model & collection](http://techbus.safaribooksonline.com/book/programming/javascript/9781430263340/chapter-4-backbone-view-and-templating-libraries/9781430263340_ch04_xhtml#X2ludGVybmFsX0h0bWxWaWV3P3htbGlkPTk3ODE0MzAyNjMzNDAlMkZzZWMyXzk3ODE0MzAyNjMzNDBfY2gwM194aHRtbCZxdWVyeT0=)

1.html
-------------
```
Constructors

define an initialize function when creating your model object

This initialize function gets called as soon as we create a new instance of the Model object. 
In this case, on creation of a new Book object, we’ll see the line “a new book” on the console.
```

2.html
-------------------

```
set Model defaults
```

3.html
---------
```
During object creation, it is possible to pass through the values of the attributes in the modelso that each instance can be unique.
```
4.html
-----------
```
You can also use the .attributes property to get a JSON object that represents all of the model data.
```
```
initialize when new Model 
Object {name: "backbone.js", date: "2014", author: "No One"}
```
5.html
-----------
set
```
initialize when new Model 
Object{
	author: "No One",
	date: "2014",
	name: "Beginning Backbone.js",
	__proto__: Object
}

````

6.html
------------
unset
```
initialize when new Model 6.html:15
Object {name: "Beginning Backbone.js", date: "2014", author: "No One"} 6.html:24
Object {name: "Beginning Backbone.js", author: "No One"}
```
7.html
-----------
clear
```
initialize when new Model 7.html:15
Object {name: "Beginning Backbone.js", date: "2014", author: "No One"} 7.html:24
Object {name: "Beginning Backbone.js", author: "No One"} 7.html:26
Object {} 
```