# Intro to Sass
There are a number of options for compiling Sass code. We can use a GUI such as Koala or scout (https://scout-app.io/) or we can use command line tools such as Node.js Sass.

## Using Koala
### Setting up
* Open Koala
* Download this repository.
  * Open *index.html* and *style.scss* in a text editor. *style.scss* is where we will write our Sass code.
* Open the web page in a browser.
* Drag the folder that contains *index.html* onto Koala.
  * Make sure you select the correct folder. Koala expects there to be a *sass* folder inside the folder you select.
* Koala should automatically detect the *style.scss* in the sass folder and generate a CSS file for you based on this *.scss* file. Check you can find this generated CSS file. It should be in a folder called css.
* Refresh *index.html* in a browser, it should now have some CSS applied.
* Take a moment to make sure you understand what has happened.
* The basic workflow is to make changes to *style.scss*. Koala will then compile this for us into plain CSS. We can then refresh the browser to see the changes.

### Re-write the CSS using Sass
Now experiment with the basic feature of Sass. Don't change the design, simply try and re-write the CSS using Sass (and the HTML) to make it more efficient.  The following link explains the basics of Sass - https://sass-lang.com/guide. Try the following:
1. Use Sass variables instead of hard coded font and colour names.
2. Can you use nesting e.g. to style the hyperlinks in the header and footer differently. Then you will no longer need the ```.contrast-link``` class.
3. Can you use ```extend``` e.g. you could extend ```content-block``` and use it in the header, footer etc. 
4. A new design requirements comes in, the news items also need rounded corners on their border, but their corners need to have a 5px radius. Can you use a mixin to generate the rounded border for both the main content areas (header, footer etc.) and the news items. 
5. Put your variables in a separate *_vars.scss* partial file. Use an *import* to load them into *style.scss*. see https://sass-lang.com/documentation/at-rules/import . Import is being phased out but, the newer methods don't work in Koala.

