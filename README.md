# UWA coding bootcamp homework week 01 - Code Refactoring
## Assignment Overview
A marketing agency has hired you to refactor an existing site to make it more accessible.

## The Website
Horiseon is a social solution services which offers technologies like SEO, Online Reputation Management and Social Media Marketing. 
It consists of an index.html file and a style.css file linked to it. The website has a navigation bar on the top right corner with three links: 

- Search Engine Optimization
- Online Reputation Management
- Social Media Marketing

Each link is anchored to their respective content below the hero image section. 
There is a side column to the right which gives information about the benefits coming with the service. 

A tabindex from 1 to 10 is also included. Below is the list of the "tabindices" in numerical order: 

1. Search Engine Optimization link in the Navigation
2. Online Reputation Management link in the Navigation
3. Social Media Marketing link in the Navigation
4. Search Engine in content
5. Online Reputation Management in content section
6. Social Media Marketing in content section
7. Lead Generation in benefits section
8. Brand Awareness in benefits section
9. Cost Management in benefits section
10. The footer



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
    - <article>
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

Made tabindex available for navigate through the webpage

Added comments
```

### style.css
``` css
Removed all unnecessary class selectors and replaced them with semantic html selectors

Removed redundant codes

Added comments
```

## The website sceen shot
![Website Screen Shot](/assets/images/Horiseon.jpg)

## Link to deployed application
https://bernardjbs.github.io/hw-boot-wk01-refactoring/
