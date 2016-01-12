# JSYG.PathDrawer
drawing interactive svg paths with [JSYG framework](https://github.com/YannickBochatay/JSYG)

##### Demo
[http://yannickbochatay.github.io/JSYG.PathDrawer](http://yannickbochatay.github.io/JSYG.PathDrawer/)

##### Installation
```shell
bower install jsyg-pathdrawer
```

##### Example
```javascript
var pencil = new JSYG.PathDrawer();

$("svg").on("mousedown",function(e) {
               
    if (pencil.inProgress) return;

    var path = JSYG('<path>');

    path.appendTo(this);

    pencil.draw(path,e);
});
```