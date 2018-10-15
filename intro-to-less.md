# Getting Started with Less

## Setting up
* Create a new folder
* Create a new HTML document e.g.
```html
<!DOCTYPE html>
<html>
<html lang="en">
    <title>Getting started with Less</title>
    <meta http-equiv="content-type" content="text/html;charset=utf-8" />
    <link href="style.css" rel="stylesheet" type="text/css">
</head>
<body>
<h1>This is a heading</h1>
<p>This is a paragraph</p>
</body>
</html>
```
* Name it *index.html*
* Create a new folder, name it *css*
* Create a *css* file, name it *style.css* e.g.
```css
body{
    color:#54869E;
}
```
Link the HTML to the CSS.
Test the page in a browser. 

## Using Less
* Navigate to this folder using the (NodeJS) Command Prompt
* You might need to set the proxy e.g.
```
npm config set proxy http://wwwproxy.hud.ac.uk:3128
```

* Enter the following to install the Less Nodejs package:
```
npm install -g less
```
* Create a new file in the css folder, *style.less*. Add the following code:
```
@muted-blue:#54869E;
body{
    color:@muted-blue;
}
h1{
    padding:10px;
    border:1px solid @muted-blue;
}
```
Back in the Command Prompt enter the following 
```
lessc css/style.less css/style.css
```
* *lessc* stands for less compile, we then need to specify the less file (*style.less*) and the output file (*style.css*).
* Refresh the page in a browser
* Have a look at *style.css* and note the changes


## Watching Less Files
Constantly have to re-compile your less files every time you make a change can be tedious. An alternative is to watch the files and compile them automatically. Again we'll use a Nodejs package to do this, one called *autoless* (https://www.npmjs.com/package/autoless). Try the following:
* In the Command Prompt enter:
```
npm install -g autoless
```
To start watching the less files enter
```
autoless css
```
* Note the output in the Command Prompt window
* Make a change to your *style.less* file
* Save it
* Note the automatic change in style.css. 
* Refresh the browser to check the changes have taken effect
* To stop watching for changes enter Ctrl+c in the Command Prompt.

## On Your Own
Have a look at http://lesscss.org/#overview for an overview of less functions. Experiment with the examples and try to get a feel for what a CSS pre-processor can do for you e.g. mixins, imports etc. 



