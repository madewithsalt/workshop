---
layout: post
title: "Data Visualization"
date: 2014-10-05 08:23:35 -0400
comments: true
summary: "Practice creating charts or graphs using data and manipulating it with a form."
categories: ["Advanced JS"]
---

The point of this exercise is to learn to read, manipulate, and visualize data in JavaScript.

- Find an interesting dataset in some sort of text format (XML, JSON, CSV, etc). 
- Store the dataset in your project folder. 
- Truncate it to a reasonable length if it’s very long (i.e. 1000 rows). Some possible sources are:
    - [explore.data.gov](http://explore.data.gov)
    - [usgovxml.com](http://usgovxml.com)
    - [geocommons.com](http://geocommons.com)
- Create an empty webpage and load the dataset into your webpage using an AJAX or JSONP request. (See slides: [AJAX/JSONP](http://www.teaching-materials.org/ajax/))
- Display the data as a `table` with columns for each of the attributes. (See slides: [HTML Tables](http://www.teaching-materials.org/htmlcss-1day/lesson3/slides.html#slide3))
- Use the [tablesorter](http://tablesorter.com/docs/) jQuery plugin to make the table sortable. (See slides: [jQuery](http://www.teaching-materials.org/jquery/))
- Create a `form` above the `table` which lets users filter or manipulate the data somehow, i.e. a dropdown box to only show rows matching a particular query, or a way of summing up attributes. Whatever would be useful with the data. (See slides: [DOM](http://www.teaching-materials.org/javascript/slides/objectsdom.html), [Events](http://www.teaching-materials.org/javascript/slides/animevents.html))
- Use the [High Charts JS library](http://www.highcharts.com/) to visualize a numerical aspect of the data. Or find [a different library here](http://selection.datavisualization.ch/).
- If the data has a geographical aspect (locations), use the [Google Maps API](https://developers.google.com/maps/) to plot it on a map. (See slides: [JS APIs](http://gdisf-js-apis.appspot.com/))
- Use [Twitter Bootstrap](getbootstrap.com) on the site to make it prettier, styling the buttons and table.
