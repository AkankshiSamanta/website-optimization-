# Website Performance Optimization


## Optimized a given Portfolio Website and a Pizza Shop Website


### About
The project aimed at optimizing an online portfolio for PageSpeed Insight score to 90 or more; and to optimize Pizza Website so that the page can render at consistent frame-rate of 60fps when scrolling.

- Clone or download repository by visiting this [GitHub](https://github.com/snehal1791/Website-Optimization) Account
- If downloading, then extract all the files.
- Open index.html on the web browser for PageSpeed of online portfolio
- Open views/pizza.html to see page render at consistent frame-rate of 60fps..


#### Part 1: Optimize PageSpeed Insights score for index.html

Optimize such that a minimum of 90 is obtained for PageSpeed Insights Score.

1. Inline the CSS in index.html
2. print.css saved as media query
3. async the google-analytics
4. Use Web Font Loader to load the Google WebFont
5. Compress jpg and png files


#### Part 2: Optimize Frames per Second in pizza.html

Optimize the speed of fps.

1. Replace all document.querySelector("#pizzaSize") with document.getElementById("pizzaSize")
2. New randomPizzas and numPizzas variables to simplify the for loop.
3. Create new variable for document.querySelectorAll(".randomPizzaContainer") and replace querySelectorAll with getElementByClassName
4. Remove sizeSwitcher() and determineDx() as no longer needed
5. Create variable to replace the querySelector with getElementById. Then append the pizza count in fragments to pizzasDiv.
6. updatePositions: sliding pizza count reduced to 48.
7. Push Math.sin(scrollConstant + (i % 5)) in phase array


### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>
