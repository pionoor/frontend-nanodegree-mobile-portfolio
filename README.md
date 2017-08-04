## Website Performance Optimization portfolio project
    A part of the Front-End Web Developer Nanodegree Program.
    
### Getting started

#### How to run

Some useful tips to help you get started:

1. Check out the repository
1. Run a local server on you PC or Mac. For Mac: 

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

1. Copy the public URL ngrok gives you and try running it through your browser.




##  Optimization

    Image compression: images were rescaled and resized to per google PageSpeed Insights.

    Inline critical CSS: critical above-the-fold content styles are inlined and applied to the document immediately vs. blocking loading. 

    Defer alternative media CSS: print stylesheets, although small, were deliberately chosen not to be served inline in HTML documents due to at least three different pages using it. A media attribute was added to ensure that it would only be downloaded when printing.

    Minifying CSS/JS: all CSS and JS files were minified--but not obfuscated--to ensure faster downloading. The formatted and indented files are still present in their respective directories, without the .min in their filenames.
        Frame rate optimization

    Loop optimization: unnecessary JS operations were pulled out of for loops wherever possible, in views/js/main.js.

   
