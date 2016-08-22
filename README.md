## Website Performance Optimization portfolio project

Project Submission - Jeff Morgan

The following link utilizes the “distributed” source code, https://jsm200.github.io/dist/ , The “dist” folder consists of code which has been minified, compressed, and optimized for optimal web user experience. 
All supporting code can be found here https://github.com/jsm200/frontend-nanodegree-mobile-portfolio . You can view code from this location or clone project repository on your machine. To do that, either clone the repository using git, or click the download zip button on the right and unzip the file. To view the optimized page, navigate to dist, then double-click index.html.
I have optimized index.html to achieve at least a 90 PageSpeed score for both mobile and desktop devices. I've optimized the JavaScript in pizza.html to achieve a frame rate of 60fps as well as reducing the time to resize pizzas in pizza.html to less than 5 ms.

Un-optimized source code is in the “src” directory.

Production code (optimized – minify, compression, etc) is in the “dist” directory.

Part 1: Optimize PageSpeed Insights score for index.html

Optimizations:

•	Reduce the size of pizzaria.jpg to 100px width
•	Inline css/style.css
•	Uglify JS
•	Minify CSS
•	Minify HTML
•	Make google-analytics script async
•	Add a media query for print.css
•	Use Web Font Loader to load the Google webfont asynchronously
•	Compress and Optimize all image files


Sources:

•	https://discussions.udacity.com/t/how-to-optimize-css-and-google-fonts/26997
•	https://discussions.udacity.com/t/gulp-and-setting-up-a-gulp-workflow-intermediate/24359
•	https://github.com/Sarika-C/frontend-nanodegree-mobile-portfolio/blob/master/views/js/main.js
•	https://discussions.udacity.com/t/p4-pizza-scrolling-rasterize-paint/30713/13
•	https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById
•	https://discussions.udacity.com/t/forced-reflow-new-issue/158305/21
•	https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByClassName
•	https://javascriptweblog.wordpress.com/2010/10/11/rethinking-javascript-for-loops/


Project Submission - Jeff Morgan - end



Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.

### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

Some useful tips to help you get started:

1. Check out the repository
1. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to the top-level of your project directory to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ./ngrok http 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!

####Part 2: Optimize Frames per Second in pizza.html

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. You will find instructive comments in main.js. 

You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).

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

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>
