Backbone.View
==================

1.html
------------

extent Backbone.View
add constructor initialize
create an instance of Backbone.View
```
View created
```
2.html
---------------

[Binding to the Physical View](http://techbus.safaribooksonline.com/book/programming/javascript/9781430263340/chapter-4-backbone-view-and-templating-libraries/9781430263340_ch04_xhtml#X2ludGVybmFsX0h0bWxWaWV3P3htbGlkPTk3ODE0MzAyNjMzNDAlMkZzZWMyXzk3ODE0MzAyNjMzNDBfY2gwNF94aHRtbCZxdWVyeT0=)

There are two ways to use el: by referencing an existing DOM element or by creating a new one.
By passing an el attribute to the constructor, you are telling the view which DOM element itshould attach to.
```
View created
<div id="sidecar"></div>
```
3.html
-----------
You can also create the el for the view dynamically by passing a number of properties to the view when constructing it.
tagName: The name of the HTML element to use for the view. If none is specified, the value of tagNamewill default to div.
className: The CSS class that will be used to render this element. This property is optional. You can specify a number of classes for the element, passing them through as space-separated values.
id: The ID to assign to the element. This property is optional.
attributes: Additional attributes to assign to the element, such as data- attributes in name-value pairs.
```
View created
<ul data-date=​"Fri Mar 21 2014 10:​55:​09 GMT+0800 (CST)​" id=​"library" class=​"libraryview">​</ul>​
```
4.html
----------
```
View created 4.html:17
begin to render 4.html:21
<div id=​"sidecar">​Hello Library​</div>​
```