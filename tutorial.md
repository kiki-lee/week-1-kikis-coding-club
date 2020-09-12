# Make a Game

## Introduction @unplugged

![Cartoon of the game at work](http://steamblender.com/wp-content/uploads/2020/09/week1gameSmall.gif)

We're going to build a game to see how many times we can click the 'A' button before time's up!

## Step 1 @fullscreen

Add a ``||info.startCountdown(10)||`` block to the onStart block to begin the countdown as soon as the game loads.

```blocks

info.startCountdown(10)

})
```

## Step 2 @fullscreen

Now add a block to sense when the 'A' button is pushed.


```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    
})
```

## Step 3 @fullscreen

Finally, add a ``||info.changeScoreBy(1)||`` block to the event block to change the score by 1 each time the 'A' button is pushed.

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    info.changeScoreBy(1)
})
```

That's it! 
Now you're ready to run the program on the emulator to the left.