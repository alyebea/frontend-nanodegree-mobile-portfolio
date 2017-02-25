# Website Performance Optimization Project

This project had two parts, optimizing index.html so that PageSpeed Insights score was 90 or greater, and optimizing pizza.html so that it ran at 60fps when scrolling and resize time on pizza slider took less than 5ms.

##How to Run

Click on index.html or visit my [GitHub Page](https://alyebea.github.io/frontend-nanodegree-mobile-portfolio/)

##Optimizations

###Mobile Portfolio

* asynchronized Google Analytics javascript and added script to perfmatter.js
* inlined CSS into index.html and eliminated link to style.css
* eliminated webfont
* compressed images and converted those that needed to be to jpeg format
* set width and height in image style tags in order to "prioritize visible content"

###Cam's Pizzeria

* optimized slider by eliminating determineDX function and simplifying for-loop by placing actual sizes rather than percentages in changePizzaSizes function
* replaced 'querySelector' with 'getElementById' or 'getElementByClass' when possible
* moved variable creation out of for-loop when possible
* changed style.left to style.transform in order to use the CSS3 translate effect
* added requestAnimationFrame to scrolling function to move javascript earlier in the frame
* added will-change and backface-visibility to style.css to place background pizzas on their own layer
* Used the height property to dynamically calculate the number of pizzas to fill the screen

##License

The project is part of the Front End Nanodegree Udacity program.
