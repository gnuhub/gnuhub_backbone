router
============

| | |
| ----- | ----- |
| |[Backbone Routers](http://techbus.safaribooksonline.com/book/programming/javascript/9781430263340/chapter-5-routers-and-events/sec1_9781430263340_ch05_xhtml) |

1.html
------------
1.html#hello

chrome console
```
Saying hello
```

```
#hello
->
routes: {'hello' : 'sayHello'},
->
sayHello: function(){
    console.log('Saying hello');
}
```

2.html
---------------


3.html
-----------

```
'hello' : 'sayHello',
'' : 'start',
'*default': 'defaultRoute'
```

```
'' is the initial route, which is an empty string
```
```
'*default' provide a default route; 
this is invoked when a URL is used that the router has not been equipped to handle. 
This route is created using the pattern *default.
```







4.html
------------

```
4.html#hello/gnuhub -> Saying hello to gnuhub
4.html -> start
4.html#hello -> Router does not handle this route
4.html#hello2/gnuhub/27 -> Saying hello to gnuhubage27
```