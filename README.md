# UXDi Programming Day

## Share Out
- What is programming and why should I care?
- Should I learn programming or should I hire someone else to do it?
- Come up with two ideas and discuss how technology could make them a reality.

## Overview of the Web
- We will talk about the request-response cycle and how this integrates with front and back end technologies.

## Introduction to HTML and CSS

##### HTML and CSS
- HTML and CSS work together to create the front end structure and design.
- Front end frameworks and the grid system.

##### Tags:
- HTML tags allow you to set up your document's structure.  
- Attributes allow you to add additional information to a tag.  
- Attributes also allow you to bridge the gap between HTML and CSS.  
- "Tags" in HTML code become "elements" on the page.  

##### Div:
- Divs are like empty rectangles.
- They help organize content on the page.

```html
<div class="margin-top-20 logo">
	My Text Inside
</div>
```

##### Semantic Elements:

- "Div" is generic.  
- HTML5 introduced other types of empty rectangles with names that mirror their purposes: header, footer, nav, etc.

![semantic html elements: header, nav, article, section, aside, footer](https://cloud.githubusercontent.com/assets/3254910/12483331/30f9061a-c009-11e5-85e6-43a447431a10.gif)

##### Input:
- Inputs allow users to enter data.
- Data is usually then saved to a database.
- Inputs come in different forms to facilitate the specific data entry type.

```html
<input type="text" class="form-control" />
<input type="password" class="form-control" />
```

##### Select list:
- Select lists allow users to select options from a dropdown menu.

```html
<select>
	<option value="USA">United States</option>
</select>
```

##### Button:
- Buttons trigger some effect - they might trigger a request to the server or change something on the current page.

```html
<button>Like this post!</button>
```

##### Anchor:
- Anchor tags are used for linking to other sites, other pages on the current site, or other parts of the current page.

```html
<a href="http://www.google.com">Google Link</a>
<a href="about.html">Link within this Site</a>
```

## CSS Stylesheets
- CSS stylesheets provide the look and feel of the website.
- There are two main ways of referencing CSS in the HTML so you can apply styles - classes and IDs.
- You can also apply styles to tags, but we try to be as specific as possible when applying styles.
- Consider this HTML:

```html
<div class="header">
	My Header
</div>
```

- Here we have a class attribute that can serve as the bridge between the HTML and CSS code.
- Here is how we would reference this class in the stylesheet:

```css
.header {
	font-size:20px;
	background-color:blue;
}
```

- We could also use IDs to reference the style:

HTML

```html
<div id="header">
	My Header
</div>
```

CSS

```css
#header {
	font-size:20px;
	background-color:blue;
}
```

- Or, using the newer header tag:

HTML
```html
<header>
	My Header
</header>
```

CSS
```css
header {
	font-size:20px;
	background-color:blue;
}
```


> **The main difference between classes and IDs is that classes can be used multiple times in the HTML document whereas IDs should only be used once.**

##### Linking CSS with HTML
- In order to run external CSS you need to link it to the HTML. This usually goes in the `head` tag:

```html
<link rel="stylesheet" href="css/style.css" />
```


## JavaScript Scripts

- JavaScript enables more user interaction with the page.
- JavaScript enables richer client interaction with a server or other services (more on this later!).

##### Key JavaScript Concepts for UX

- "Events" like hover, click, and page load drive most JavaScript behaviors.
- AJAX allows client-server interaction to happen in the background.

##### Linking JS with HTML  
- In order to run external JS you need to link it to the HTML. This usually goes before the closing `body` tag:

```html
<script src="js/app.js"></script>
```

## HTML Markup Lab
- Open the `html_form` folder and open `index.html`.
- For each comment denoted by `<!-- -->` replace the comment text with the correct HTML as per the instruction to create the form.
- Alter the CSS file to use a Google Fonts font. You will need to use the `font-family` CSS property.
- Bonus: Use CSS to change the background color of the page. Experiment with using images as backgrounds as well.
- Double Bonus: Review the CSS `transition` property documentation and try to create a small animation anywhere on the form. An example may be to highlight a border around a form field when it is clicked.

## A Little More on CSS
- CSS is a powerful language and has an easy-to-learn syntax.
- CSS can be used to achieve everything from pixel-perfect colors to advanced animations.
- If you want to see a couple examples, check these out:
	- [http://codepen.io/juliangarnier/pen/idhuG](http://codepen.io/juliangarnier/pen/idhuG)
	- [http://www.rleonardi.com/interactive-resume/](http://www.rleonardi.com/interactive-resume/)

## CSS Colors
- There are three main ways to use colors in CSS - semantic, HEX values, and RGB(A) values.

##### Semantic:

```css
div {
	background-color:black;
}
```

##### HEX:

```css
div {
	background-color:#000000;
}
```

##### RGBA:

```css
div {
	background-color:rgba(0,0,0,0.5);
}
```

## CSS Gradients
- CSS gradients were introduced as of CSS3.
- They allow for a gradient of colors to be applied across multiple solid colors.
- These are hard to write via raw CSS, so generators are often used.
- Let's have a look at one [here](http://www.colorzilla.com/gradient-editor/).

## CSS Color Lab
- Create three divs via Codepen with a width, height, and border.
- Style them all differently via classes or ids (your choice) by giving them varying colors or background colors, using a different method each time.
- Add a gradient to at least one of the divs.

## Putting it Together
- For this lab we will be creating a personal landing page using HTML and CSS.
- A starter page has been created for you [here](about_me_starter_website/).
- This is meant to be creative, but make sure to at least do the following:
	- Add the class "fixed-top" to the header to make it stay in place during scroll.
	- Use rgba colors to make the header navbar semi-transparent.
	- Use Google Fonts to implement a font of your choice for the logo.
	- Replace the picture of Arun with one of you. You will need to look up the <img> tag to make this happen.
	- Replace the picture of the motorcycle with a background of your choice (Hint: Have a look at the CSS to find out where this background comes from).
	- Make the background of the banner have a parallax effect. Hint: Research the "background-attachment" property in CSS.
	- Change the text throughout the page to reflect your own personal information.
	- Add a gradient to the background of the user-info-text class in CSS.
	- **Bonus:** Implement a small animation using CSS somewhere on the page. You may want to research the `transition` and `transform` CSS properties.
- We will be discussing how to make this web page live using a service called BitBaloon.

## Overview of Back End Development

##### Introduction
- Why is a back end needed?
- How does the back end interact with the front end? 
- APIs and services.
- Back end language examples:
	- Ruby (Ruby on Rails)
	- PHP
	- Python (Django)
	- JavaScript (NodeJS)

##### Databases
- Difference between SQL and NoSQL databases.
	- MySQL
	- PostgresSQL
	- MongoDB
	- Redis

## Architecture Design Lab

Let's look at some popular sites and determine what technologies could be used. Think about the interaction between backend and frontend and how they fit together.

Your answer doesn't have to be the "right" one (the technology they actually use), but we just want you to demonstrate you understand how each piece fits together. You can choose your own site to analyze, but here are some examples:

- Twitter
- Facebook
- Instagram
- Medium

## Introduction to Algorithms
- Algorithms are step-by-step procedures for various calculations.
- They are generally used for data processing and automated reasoning.
- Algorithms are used in programming to perform calculations useful to the application.
- Examples of algorithms:
	- Search for values in a database by location.
	- Find the shortest path between two points.
	- Determine the most popular songs for a given demographic.
	- Suggest friends that you may know based on certain criteria.

## Algorithm Lab
- In groups of 3-4 think of how we may accomplish the above algorithms using programming.
- You definitely don't need to come up with any code, but just think conceptually as to how these could be solved.
- Draw out your concepts visually.