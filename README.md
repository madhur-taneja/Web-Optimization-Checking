# Website Performance Optimization portfolio project

Open and view the Project at: [Website Optimization Checking](https://madhur-taneja.github.io/Web-Optimization-Checking/)

## Getting started

#### Tools required:

* [CSS Minifier](https://cssminifier.com/)
* [JS Minifier](https://javascript-minifier.com/)
* [Kraken.io](https://kraken.io/) and [Optimizilla](http://optimizilla.com/)
* [PageSpeed Tools](https://developers.google.com/speed/pagespeed/insights/)

#### Steps to run the app:
> Open the project through the `hosting link` provided above or through the `.zip` file provided and extract file.
> To open `index.html`:
* Open the main folder.
* Open `index.html`.
> To open `pizza.html`:
* Open `view` folder in main folder.
* Open `pizza.html` in `view`.
* `pizza.html` can also be opened through `Cam's Pizzeria` link in `index.html`.
> To open `main.js`:
* Open `js` folder in `view` folder.
* Open `main.js`.

## Part 1: Optimize PageSpeed Insights score for index.html

* The aim of this project was to optimize index.html to a pageinsight speed score above 90.
* My score was: 95 for Mobile and 96 for Desktop version.

### Step 1: Optimizing `index.html`
> Unlinking style.css and making it internal after minifying it.
> Using media query "print" on print.css.
> Shifting script tags from head to end of body and using async attribute on them.

## Part 2: Optimize Frames per Second in pizza.html
* The aim of this project was to optimize pizza.html to 60 fps scrolling speed.

### Step 1: Optimize `pizza.html`
> Shifting script tags from head to end of body.

### Step 2: Optimize `main.js`
> Minified js for arrays.
> Changes in changePizzaSizes()
* Declaring rPC and dx outside the loop as it was being declared again and again.
> Changes in `UpdatePosition()` function.
* Declaring phase outside the loop as it was being declared again and again.
> Changes in `document.addEventListener()`.
* Reducing the number of times the loop runs as image will be generated lesser number of times.