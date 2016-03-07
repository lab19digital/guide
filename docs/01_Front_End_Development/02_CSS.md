It goes without saying that you should use a CSS preprocessor like Less, Sass or Stylus to keep your code DRY and maintanable. You should setup vars for anything that repeats throughout the script like colours, margins, widths, padding, etc. 

Prefer splitting your code up into components, and look to using the BEM approach so that your rules aren't nested too deep within the hierarchy and you don't end up with problems from cascading. 

[http://getbem.com/introduction/](http://getbem.com/introduction/)

It's beneficial for many reasons to use a CSS framework like Bootstrap which also comes with grids built in and many components already styled. Then you're able to customise a set of variables and make adjustments without having to reinvent the wheel.