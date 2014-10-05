---
layout: post
title: "YouTube Player"
date: 2014-10-05 08:32:21 -0400
comments: true
summary: "Work with YouTube's JSON API."
categories: ["Advanced JS"]
---

In this exercise, you'll try to bring in Youtube video information using their JSON API. You may find [these slides](http://gdisf-js-apis.appspot.com/) useful.

Start with [this file](http://www.teaching-materials.org/ajax/jsapis_solution.html).

- Go to the [Youtube API docs](https://developers.google.com/youtube/2.0/developers_guide_jsonc) and read through them. Look at the sample output and the example URLs for the API. Find a URL that will give you search results, and test that out in the browser.
- The webpage currently brings in video information using the jQuery `$.ajax` function to bring in a local `videos.json` file into the page. 
- Change that function so that it instead brings in the results of a Youtube API search from the Youtube servers and displays those results instead. Search for whatever you fancy, but limit the search to 5 results. 
- **Tips:** Remember that the JSON that the Youtube API returns will be different than the JSON format of `videos.json`. You should `console.log` inside your callback to see what the data looks like and make sure you're using it correctly. In particular, check how they store the `ID`, the `author`, and the `rating`.
- **Bonus:** Create your own playlist on Youtube of your favorite videos, and bring that into the page instead.
- **Bonus:** Add a search button to the page so that people can search for any query.

Make sure that you use your browser developer tools to make debugging easier while working on this. Check for errors, and use `console.log()` to figure out how far your code makes it, and what the values of your variables are along the way.