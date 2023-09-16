# Sass

It stands for Syntactically Awesome Style Sheets. SASS is an extension of CSS and also a popular CSS pre-processor. It is compatible with all CSS versions.

### Operators

Provides standard math operators. These operators can be used inside our css code directly.

Example: h2 {  
 font-size: 5px \* 2px; // can only be used in SCSS  
 }

### Variables

Sass variables are used to store information. We can add background-color, font-style or any CSS according to future requirement in the code.
Also, like PHP, $ is used to declare a variable.

    Example:  $primary-color: white;

              body{
                color: $primary-color;
              }

### Nesting

In Sass, we can combine multiple CSS rules within one another. If you are using multiple selectors, then you can use one selector inside another to create compound selectors.

    Example:  .container{
                h1{
                 font-size: 25px;
                 color:#E45456;
                }
               }

### Mixin

It helps to make groups od CSS declarations that are used repeatedly and we can even pass values/parameters according to our needs.
The mixin can store multiple values or parameters and call function to avoid writing repetitive codes. Mixin names can use underscores and hyphens interchangeably.

    Example:  @mixin border-radius($radius) {
                -webkit-border-radius: $radius;
                -moz-border-radius: $radius;
                -ms-border-radius: $radius;
                 border-radius: $radius;
              }

              .box { @include border-radius(10px); }

### Partials

@import directive allows us to include the content of one file in another. It includes the file in the CSS.

    Example:  @import filename;
