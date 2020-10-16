# CSS Pre-Processors and CSS Libraries

There are a number of options here. If you are familiar with using command line tools and Node.js there is Node.js implementation of Sass see https://sass-lang.com/install.

Alternatively you can use an application with a graphical user interface to compile Sass code. There are several different applications out there. The instructions below describe the use of Koala, it's free and easy to use.

## Getting Started with Sass and Koala

### Setting up
* Download and install Koala - http://koala-app.com/
* Download this repository.
  * Open *index.html* and *style.scss* in a text editor.
    *style.scss* is where we will write our Sass code.
* Open the web page in a browser. Note that at the moment it doesn't have any CSS applied to it.
* Open Koala.
* Drag the folder that contains *index.html* onto Koala.
* Koala should automatically detect the *style.scss* in the sass folder.
* Right click on *style.scss* and select compile.
* Koala should generate a CSS file for you based on the *.scss* file. Check you can find this generated CSS file. It should be in a folder called css.
* Refresh *index.html* in a browser, it should now have some CSS applied.
* Take a moment to make sure you understand what has happened.
* The basic workflow is to make changes to *style.scss*. Koala will then compile this for us into plain CSS. We can then refresh the browser to see the changes.

### Re-write the CSS using Sass
Now experiment with the basic feature of Sass. Try the following:
1. Use Sass variables instead of hard coded font and colour names.
2. Put your variables in a separate *_vars.scss* partial file. Use an *use* to load them into *style.scss*.
3. Experiment with using mixins, nesting and extends. You should be able to re-use CSS rules and reduce the number of classes used in the HTML page. Try and make your CSS efficient and easy to maintain.

The following link explains the basics of Sass - https://sass-lang.com/guide.

## CSS Libraries and Frameworks
* Have a look on the lecture slides. Find a library (e.g. Animate.css) you might want to use for your assignment.
* See if you can create a simple example that uses the library.
* Next pick a framework e.g. Bootstrap. Again, see if you can create a simple example that uses the framework.
* Compare the two approaches libraries vs frameworks.
* How easy do you think it will be to create a unique design for a website if you use the library/framework.
