Website Optimization Project
===============================
The portfolio presented in this application displays a set of different projects completed by Cameron P. Both the homepage and Cam's Pazzeria were in need of optimization in order to run at an acceptable performance level. This has been achieved via the use of chrome dev tools timeline component, google pagespeed insights and font squirrel webkit generator.

#Getting Started#

##System Requirements##
The portfolio application uses HTML5, Javascript and CSS. In order to use this application, please ensure that you are using a modern browser which supports these technologies. If you need a new browser you can find Chrome here: [Google Chrome](https://www.google.com/chrome/browser/desktop/). Please also ensure you have an stable internet connection and the application uses data provided by various other websites.

##Installiation##
The portfolio application does not require any executable installation, in order to install the application, all you need to do is place a copy of the application files from the [github respoitory](https://github.com/rosso007/website-optimization) on your computer.

##Using the application##
In order to start using The portfolio, ensure you have an internet connection and navigate to the application files to open the Index.html file.

Once the page is loaded and you can see the the application on screen, you can start navigating through the index page and Cam's Pizzeria page.

##Optimisations List:##
1. Added a print media query to allow the print.css file to be using only in print viewport.
2. Changed http://www.google-analytics.com/analytics.js and perfmatters.js to load asynchronously.
3. Removed the google webfont call to improve performance and instead loaded from a local store in the CSS directory.
4. Added a script to optimize the CSS delivery for stylesheet.css and style.css.
5. Minified all images within the website to reduce filesize.
6. Inlined all the critical path CSS from style.css into index.html and pizza.html to increase performance.
7. Moved changeSliderLabel, sizeSwitcher, determineDx & changePizzaSizes functions out of the nested structure to reduce function runtimes.
8. Changed querySelectorAll to be getElementsByClassName to reduce scripting times.
9. Stored 'document.getElementsByClassName("randomPizzaContainer")' within a container variable to only fetch it once rather looping through.
10. Moved 'var dx' and 'var newwidth' outside of the for loop to stop the repeated creation of these variables.
11. Moved 'Var items' out of the function scope to allow this to load prior to the function call.
12. Created 'var scrollTop = document.body.scrollTop;' within the update positions function to increase performance of the function.
13. Created a 'phaseValues' array to store the phases calculated and only calculated enough values to capture all distint values. Rather than iterating through the loop 200 times.
14. Reduced the number of items created to be about 40 from 200 as this is more than what is shown on page at one time.
15. Added backface-visibility: hidden; CSS to the mover class to increase framerate of scrolling.
16. Created a minified and resized pizzeria image for index.html.