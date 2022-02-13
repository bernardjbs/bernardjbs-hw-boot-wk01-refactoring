# UWA coding bootcamp homework week 01 - Code Refactoring
## Assignment Overview
A marketing agency has hired you to refactor an existing site to make it more accessible.

## The Website
Horiseon is a social solution services which offers technologies like SEO, Online Reputation Management and Social Media Marketing. 
It consists of an index.html file and a style.css file linked to it.

## The Assignment
As a requirement to this assignment, the changes I make must not affect the design of the website. The goal of this refactor is to change the codebase so that it follows the accessibility standards and be optimized for search engines. 

## The Changes
### index.html
``` html
Added meaningful title 
<title>Horiseon Social Solution Services</title>

Added a <main> tag

Added alt attirbutes to all <img> tags

Replaced <div> tags with the following semantic html tags: 
    - <header>
    - <nav>
    - <section>
    - <footer>

Id to content was missing
<div id="search-engine-optimization" class="content-item">

since all "items" are using the same style in the content section, 
replaced all classes names to "content-item"
<div id="search-engine-optimization" class="content-item">
<div id="online-reputation-management" class="content-item">
<div id="social-media-marketing" class="content-item">

since all "items" are using the same style in the benefit section, 
replaced all classes names to "benefit-item"
<div class="benefit-item">   

Added comments
```

### style.css
``` css
Removed all necessary class selectors and replaced them with semantic html selectors

Removed redundant codes

Added comments
```