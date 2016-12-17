# Nanodegree Project: Website Optimization

## Summary
Improved website performance as measured by Google Pagespeed Insights.

### How to load the mobile site
After cloning or downloading the directory from GitHub, the biggest challenge to getting the mobile site up and running is starting the web server.  I've found python to be the easiest way to get a web server up and running.  These instructions assume you'll use python.  If you have the ability to start up a different web server, then you're all set.    
  
  - ( 1) open a command prompt
  - ( 2) type ```python --version``` and press enter
  - (3a) if you are told that python is not recognized, then you must install python
  - (3b) if you are given a python version number, then you are ready to run the server
  - ( 4) after you have python installed (and ```python --version``` produces a version number in the output within the command prompt) navigate (using your system's change directory command) to the directory where you've saved the mobile site code--  you want to start your server from within the same folder where index.html resides.
  - ( 5) now that you've navigated to the mobile site's main directory, depending on which version of python you have installed, type one of the following commands:

* If using Python 2
```sh
python -m SimpleHTTPServer [port number]
```      
* If using Python 3
```sh
python -m http.server [port number]
```
* I typically run ```python -m http.server 1234```, which produces the following message:
```sh
Serving HTTP on 0.0.0.0 port 1234
```
- ( 5) The final step is to open your browser and enter the following URL:
```sh
http://127.0.0.1:1234
```
Avoid using http://localhost:1234, "localhost" caused issues with API calls.



## Testing Site with Pagespeed Insights
- I found it easiest to use GitHub to host my site (robeddy.github.io) and test the PageSpeed.  
- Simply upload your code to [username].github.io.
- Submit your github.io url to the PageSpeed Insights page.

## Modifications to main.js

1. Delete determineDx function
2. Modified changePizzaSizes function
3. Removed the function generator
4. Modified function randomname
5. Added requestAnimationFrame to updatePositions
6. Changed all document.querySelectorAll to document.getElementsByClassName or document.getElementsByID
7. Modified updatePositions function
