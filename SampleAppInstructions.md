_This instruction sheet was adapted from the [Greedy Chef app](https://mcbeckster.makes.org/thimble/NTc4NjgzMTM2/chef-adventure-game), recreated here to make it a little more printable._

#Basic Chef Game

**GOAL**: To become familiar with AppMaker, particularly
* Adding bricks to your app
* Customizing bricks
* Connecting bricks
* Adding pages and what to use additional pages for
* How to publish and save your app

**STRUCTURE**: Two page app - a start button page, and a page with the with game, gamepad and counter. 

##The steps

###Set up the app

Images        | Instructions
------------- | -----------------
![step1](http://i.imgur.com/6cDoJ1S.png) | 1. Open [Appmaker](https://apps.webmaker.org/designer). On the first first page, add the following bricks in this order: Header brick, Image brick, Button brick. These bricks are listed on the left hand side of the screen. 
![step1b](http://i.imgur.com/EpQEuQw.png) | Click on each brick and use the Customisation toolbar on the right to edit your bricks. Change the image to whatever image you'd like, choose an app title, or customise the brick colours. 
![step2](http://i.imgur.com/ZWImSnL.png) | 2. Add a new page to your app. Add the following bricks in this order: Counter brick, Chef Adventure brick, Game Controller brick. 
 | The Counter brick will keep track of how many items you've picked up, and you can customise the units (pies, eggs, cats, etc). 
 | The Chef Adventure brick is where gameplay will happen - more on how to customise this brick below. The Game Controller brick is already edited to work in the most straight-forward way, so there's no need to customise this brick.
![step3](http://i.imgur.com/lSsLlRe.png) | 3. **The Chef Adventure Brick**. This brick offers you lots of options. You can change the floor, build walls, and add items for your chef to pick up.
 | Click on the brick and you'll see these options appear below. Select different floor/wall/item options to customise your game. Click on the erase box to make changes to what you've built. Play around with the different options until you're happy with the results. 
 | **Note**: Check out the chef in the top left hand corner of the image; this is where your chef is going to start the game, so be sure not to put a wall in his way!

###Connect the bricks

Images        | Instructions
------------- | -----------------
no image | 1. Connecting the bricks involves assigning bricks to a channel (A, B, C, D, etc.), and linking them to other bricks in the app. This step is what makes the app functional.
![step2](http://i.imgur.com/DFhmwIc.png) ![step2a](http://i.imgur.com/YMKeIgj.png?1) | 2. Click on your first page. Only one brick on this page needs a channel: the "Start" brick. We want to click on this brick to initate the game. Click on the output arrow on the right side of the brick, and assign it to 'A' channel. Open Page 2 of your app and select the Chef Adventure brick's input arrow on the left of the brick. Assign 'A' channel to 'entertile'. Doing this will ensure your chef enters the game.
![step3](http://i.imgur.com/k495d0Z.png) | 3. Connecting the rest of the bricks on page 2 looks complicated, but each step is explained below. We're almost there!
 | * Channel B: This channel will alert the counter that a coin has been collected. Click on the output arrow on the right of the Chef Adventure brick. Assign 'B' channel to "An object stepped on." Connect this brick to the counter by clicking on the input arrow on the left of the Counter brick. Assign 'B' channel to "Count Up."
 | * Channel C: Let's connect the game controller to the game. Click on the output arrow on the right of the game controller, and assign 'C' channel to "Any button pressed." Connect this brick to the game by clicking on the input arrow on the left of the Chef Adventure brick, and assign 'C' channel to "buttonpress."
 | * Channel D:When the chef collects items, we need that item to be removed from the game. To do this, click on the output arrow on the right of the Counter brick, and assign 'D' channel to "Current Count." Connect this brick by clicking on the input arrow on the left of the Chef Adventure brick, and assign 'D' channel to "Destroy Object."

###Publish and play your game

1. **Share**: Now that you've created an awesome app, sign-in to or create a Webmaker account and select "Publish" from the "App" drop-down menu. Share your link with your friends and family, on Facebook and on Twitter, tweet @MozillaAppmaker
2. **Download the app to your mobile device**: You can install Appmaker apps on your mobile device and use it on the go. Once you publish the app, you can have a link to the app emailed to you or use a QR reader to take a picture of the code.
 