# Make a Game

## Introduction @unplugged

![Cartoon of the Rock Paper Scissors game](/static/mb/projects/a4-motion.png)

We're going to build a game to see how many times we can click the circle before time's up!

## Step 1 @fullscreen

Add a ``||input:on shake||`` block to run code when you shake the @boardname@.

```blocks
input.onGesture(Gesture.Shake, () => {

})
```

## Step 2 @fullscreen

Add a ``hand`` variable and place the ``||variables:set hand to||`` block in the shake event.

![A animation that shows how to create a variable](/static/mb/projects/rock-paper-scissors/newvar.gif)

## Step 3 @fullscreen

Add a ``||math:pick random||`` block to pick a random number from `1` to `3` and store it in the variable named ``hand``.

```blocks
let hand = 0;
input.onGesture(Gesture.Shake, () => {
    hand = randint(1, 3)
})
```

In a later step, each of the possible numbers (`1`, `2`, or `3`) is matched to its own picture. The picture is shown on the LEDs when its matching number is picked.
