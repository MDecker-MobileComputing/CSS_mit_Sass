# Fluid Layout with Sass #

This repository contains an example of how to use the alternative stylesheet language [Sass](https://en.wikipedia.org/wiki/Sass_(stylesheet_language))
for an HTML page with a *Fluid Layout* (which is one of the core techniques for *Responsive Web-Design*).

<br>

----

## Direct View ##

The HTML file in this repository can be viewed directly at [this URL](https://mdecker-mobilecomputing.github.io/CSS_mit_Sass/index.html).

<br>

----

## Generate the CSS file ##

Install [Sass](https://www.npmjs.com/package/sass) using the *Node Package Manager*:
````
  npm install -g sass
````
The option `-g` installs the package globally, so the program `sass` can be called from different folders on the computer and is not included into the project folder (because it is not needed during runtime).

<br>

Invoke *Sass* to convert the `scss` file into a `css` file that can be included by the `html` file:
````
  sass --no-source-map --style=compressed MeinStylesheet.scss docs/MeinStylesheet.css
````

<br>

This command is defined in this repo's file `package.json` as script with the name `bauen` (German for "build"), so you also invoke it as follows:
````
  npm run bauen
````

<br>

There are also other Sass processors, e.g. [node-sass](https://www.npmjs.com/package/node-sass).
