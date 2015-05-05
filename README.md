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

## Events suported.

- enterFrame
- removed
- load
- mouseMove
- mouseUp
- mouseDown
- mouseOver
- mouseOut
- releaseOutside
- click
- mouseWhell
- rollOut
- rollOver
- rightClick

## Alias

- $click = $bind('click');
- $hover([function mouseOver],[function mouseOut]) = $bind('mouseOver')
- $mouseOver([function mouseOver],[function mouseOut]) = $bind('mouseOver')
- $mouseMove = $bind('mouseMove');
- $mouseOut = $bind('mouseOut');
- $mouseUp = $bind('mouseUp');
- $enterFrame = $bind('enterFrame');
- $mouseDown([function mouseDown],[function release || releaseOutside]) = $bind('mouseDown')

---------------------------------

The MIT [License](https://raw.githubusercontent.com/webcaetano/jinx/master/LICENSE.md)
