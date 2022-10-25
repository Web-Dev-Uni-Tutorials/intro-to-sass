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

## Using Sass with Node.js
If you aren't familiar with using command line tools, have a look at [Intro to the Command Prompt](intro-to-command-prompt.md) which explains the basics.

### Installing a Node.js version of Sass
* Open the Node.js Command Prompt (it must be the Command Prompt)
  * If you are doing this at home, you won't have a special Node.js Command Prompt and you can just use your regular Command Line interface e.g. Powershell. 
* Enter the following:

```
npm install -g sass
```

This installs the sass package. The *-g* flag specifies it should be installed globally so it will be available for all projects on the machine.

## Using node Sass
* Using the Command Prompt navigate to a web application folder where you have some Sass code
* In the Node.js command prompt, enter the following:
```
sass --watch sass/style.scss css/style.css
```
* This will look for a Sass file in a folder called *sass*, compile it and output it to a *css* folder. You might have to modify the above code for your file names, but if you've previously done the Koala Sass practical the naming should be the same.
* Make changes to your Sass file. You should get some feedback through the Command Prompt and *style.css* should update.
* Previously we used Koala. One limitation of Koala is that is doesn't use the most up to date version of Sass e.g. we had to use *@import* to combine multiple stylesheets. Have a look at the *@use* rule (https://sass-lang.com/documentation/at-rules/use) which is a better way of doing the same thing. Modify your Sass code to use *@use*.
* Once you've finished, in the Command Prompt enter *ctrl+c* to stop watching the Sass code.
