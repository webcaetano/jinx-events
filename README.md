# [![Imgur](http://i.imgur.com/FHjshUv.png)](https://github.com/webcaetano/jinx)

[Jinx](https://github.com/webcaetano/jinx) module for chaining prototype events

Example
```javascript

var myMc = new foo();

myMc.x = 250;
myMc.y = 100;
addChild(myMc);

myMc.$bind('enterFrame',function(){
	this.rotation+=0.5; // it will spin
}).$bind('click',function(){
	this.y+=5; // it will go down a when clicked
}).$hover(function(){
	this.alpha=0.5; // it will be 50% alpha when mouse hover
},function(){
	this.alpha=1; // it will be 0% alpha when mouse out
})

```

Events suported.



---------------------------------

The MIT [License](https://raw.githubusercontent.com/webcaetano/jinx/master/LICENSE.md)
