---
layout: post
title: "Memory Game"
date: 2014-10-04 16:44:32 -0400
comments: true
summary: "Practice Arrays, Events, Functions, and working with the DOM with this memory card game."
categories: ["Advanced JS"]
---

# The Memory Game

In this exercise, you'll make a LOLCat memory game -- you can see a screenshot of a sample solution on the right. A memory game consists of an even number of tiles with images on one side and a generic back. Each image appears on precisely two tiles. You start the game with all tiles turned face down, and proceed to flip over two tiles at a time. If the two tiles have the same image, they remain face up. If not, they're flipped face down again after a short delay. The goal of the game is to get all the tiles flipped face up (i.e., find all the matching image pairs) in the least number of tries.

{% img /images/posts/beg_js/memory1.png %}  
_Example of what we're building._

We'll make the game more fun by using random LOLCat images from [http://lolcat.com](http://lolcat.com) for the tiles. This site works particularly well for our purposes because their images follow a regular naming scheme so we can avoid scraping image URLs from sites by hand. The lolcat.com image URLs follow the pattern `http://lolcat.com/images/lolcats/NNNN.jpg`, where `NNNN` is a sequentially assigned number. Some experimentation shows that most of the range between `900` and `1250` works well, though a few of the images are missing. (If you happen to pick a missing one, it'll appear as a broken image as show in the example -- don't worry about it, or just reload your page to pick another set.)

## Here are some suggested steps for building the game:


Write the HTML for the game's page, displaying a grid of face-down tiles. You can use any image you want for the tiles' backs, but make sure it's not easily confused with the LOLCat pictures, so it's clear whether a tile is face up or face down. 

You'll probably want to use a `<table>` to lay out the tiles, and set the width and height of each image by hand. You can either write the table by hand into your HTML file, or write code to generate it dynamically using `document.createElement` and `appendChild`.

Write code to pick a bunch of random LOLCat image URLs and stick two copies of each URL into an array, then randomize the order of the array (using the code from the previous exercise). 

You might also take this opportunity to preload the images so there'll be no delay when they're flipped over for the first time. Make the preload images visible for now so you can verify that you're forming the URLs correctly.

Assign one LOLCat URL from the randomized array to each tile. The easiest way to attach the URLs is to store them in a made-up attribute (e.g. facesrc) right on the DOM image elements. 

The browser will ignore any attributes it doesn't understand, but you'll be able to retrieve them later in your code when handling click events on the elements. (Note though that Firebug will not show your custom attribute in the DOM pane.)

Attach a `click` handler to each tile that will turn it face up. Make sure that clicking on tiles that are already face up does nothing.

Add a `timeout` handler when a tile is turned face up that will flip the tile face down again after a short delay (e.g., 500 milliseconds).
Add the game logic that keeps track of the tiles that are face up and reacts appropriately based on whether they match or not.

You should now have a working game! Have fun playing it and tweaking it to really make it your own. 

**Here's a few suggestions for extra features you could add:**
  - Add an outline around "active" tiles (flipped up but not yet matched) so it's clear which tile the player is currently trying to match.
  Add a timer or move counter to make the game more competitive. (For the timer, window.setInterval() could prove useful.)
  - When the game is over, allow the player to see the full-size LOLCat pictures from the tiles.
  - Allow the player to start a new game with a button, rather than by reloading the page. You could also allow them to pick the size of the board to play on.
  - Manually make a list of "bad" image numbers in the code to avoid picking them, or find a different source of pictures to play with.


