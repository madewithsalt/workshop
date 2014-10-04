---
layout: post
title: "Media Queries"
date: 2014-10-04 11:28:00 -0400
comments: true
summary: "Use CSS Media Queries to change the look of a webpage when it resizes, and when it's printed."
categories: ["Advanced CSS"]
---

# CSS: Media Queries Exercise
The goal of this exercise is to use CSS media queries to make a webpage appeardifferent for printing and for different window sizes.

Start with [this webpage](http://www.teaching-materials.org/csstools/exercise_media_before.html), which already has HTML and CSS for a header, navigation, content, sidebar, and footer. This is what it looks like:
{% img /images/posts/html_css/media_queries1.png %}


## Print Media Queries
Add a CSS media query and appropriate styles so that the webpage looks like the screenshot below when printed. 

{% img /images/posts/html_css/media_queries2.png %}

### Specifically:
_The header, navigation, and footer should be hidden.  
The sidebar should display under the main content._


## Size Media Queries
Add a CSS media query and appropriate styles so that the webpage looks like the screenshots below when resized to smaller widths. 

### Specifically:
- The sidebar should be hidden.
- The body should have no padding.
- The images shouldn't exceed the width of the window.
- The navigation items should each be on their own line.
- The header should be fixed, so that it stays at the top after scrolling.

### Examples:
{% img /images/posts/html_css/media_queries3.png %}

