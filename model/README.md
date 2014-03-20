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
8.html
-----------
clone
```
initialize when new Model 8.html:15
Object {name: "Beginning Backbone.js", date: "2014", author: "No One"} 8.html:24
Object {name: "Beginning Backbone.js", author: "No One"} 8.html:26
initialize when new Model 8.html:15
Object {} 8.html:29
Object {name: "Beginning Backbone.js", author: "No One"} 
```

Attribute Function Reference
-------------------------------------

| Operation | Description |
| ---------- | ----------- |
| .get(<attribute name>) | Returns the value of the attribute with the given name. If no such attribute exists, undefined is returned. |
| `.set(<attribute name>, <attribute value>)` | Sets the value of the given attribute to the value provided in the second parameter. If the attribute doesn’t already exist, a new attribute is created with this value. |
| .has(<attribute name>) | Checks for the existence of the given attribute in the model object. |
| unset(<attribute name>) | Removes an attribute from the model, if it exists. |
| clear() | Removes all attributes from the model object. |
| .attributes | Returns a JSON representation of all attributes in the model. |
| .clone() | Creates a new instance of the model with all the same attributes. |