# Getting Started with Sass and Koala
There are a number of different ways to use Sass. In this practical we will use Koala as it is an easy way to get up and running with Sass.

## Setting up
* Download the repository
  * Open *index.html* and *style.scss* in a text editor
* Open the web page in a browser. Note that at the moment it doesn't have any CSS applied to it.
* Open Koala
* Drag the folder that contains the web page and scss folder into Koala
* Koala should automatically detect the style.scss file
* Right click on the style.scss and select compile
* Koala should have generated a CSS file for you based on the Sass file. Check you can find this generated CSS files.
* Refresh *index.html* in a browser it should now have some CSS applied.
* The basic workflow is to make changes to style.scss. Koala will then compile this for us into plain CSS . We can then refresh the browser to see the changes.

## Re-write the CSS using Sass
1. Use Sass variables instead of hard coded font and colour names.
2. Put your variables in a separate *_vars.scss* partial file. Use an *import* to load them into *style.scss*.
  * Recently Sass have made their use of partials much more sophisticated to use *modules*.
  * This won't work when using Koala at university as it is running on an older version of Sass. We have to use the *import* feature https://sass-lang.com/documentation/at-rules/import
3. Experiment with using mixins, extends and placeholders. You should be able to re-use CSS rules and reduce the number of classes used in the HTML page. Try and make your CSS efficient and easy to maintain.

The following link should explain the basics of Sass - https://sass-lang.com/guide.
