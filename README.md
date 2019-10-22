# CSS Pre-Processors and CSS Libraries

## Getting Started with Sass and Koala
There are a number of different ways to use Sass. In this practical we will use Koala, an easy way to get up and running with Sass.

### Setting up
* Download the repository.
  * Open *index.html* and *style.scss* in a text editor.
    *style.scss* is where we will write our Sass code.
* Open the web page in a browser. Note that at the moment it doesn't have any CSS applied to it.
* Open Koala.
* Drag the folder that contains *index.html* and the sass folder onto Koala.
* Koala should automatically detect the *style.scss* file.
* Right click on *style.scss* and select compile.
* Koala should generate a CSS file for you based on the *.scss* file. Check you can find this generated CSS file.
* Refresh *index.html* in a browser, it should now have some CSS applied.
* Take a moment to make sure you understand what has happened.
* The basic workflow is to make changes to *style.scss*. Koala will then compile this for us into plain CSS. We can then refresh the browser to see the changes.

### Re-write the CSS using Sass
Now experiment with the basic feature of Sass. Try the following:
1. Use Sass variables instead of hard coded font and colour names.
2. Put your variables in a separate *_vars.scss* partial file. Use an *import* to load them into *style.scss*.
    * Recently Sass have made their use of partials much more sophisticated to use *modules*.
    * This won't work when using Koala at university as it is running on an older version of Sass. We have to use the *import* feature https://sass-lang.com/documentation/at-rules/import
3. Experiment with using mixins, extends and placeholders. You should be able to re-use CSS rules and reduce the number of classes used in the HTML page. Try and make your CSS efficient and easy to maintain.

The following link explains the basics of Sass - https://sass-lang.com/guide.

## CSS Libraries and Fraemworks
* Have a look on the lecture slides. Find a library e.g. Animate.css you might want to use for your assignment.
* See if you can create a simple example that uses the library.
* Next pick a framework e.g. Bootstrap. Again, see if you can create a simple example that uses the framework.
* Compare the two approaches libraries vs frameworks.
* How easy do you think it will be to customise the library/framework to create a unique design for a website. 
