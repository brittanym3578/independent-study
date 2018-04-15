# Entry 3:
## New Discoveries with SASS
<img src = "https://alistapart.com/d/_made/d/ALA340_SASS_300_960_501_81.jpg"/>
Photo Credit: https://alistapart.com/article/getting-started-with-sass
## Importing 
You can make a SCSS file from partial SCSS files. To use a partial SCSS file in
another SCSS file, you use `@import` and next to it write the name of the partial
file in single quotes. When a SCSS file that contains `@import` gets turn into a 
CSS file, the CSS file will have the properties of the partial file.

#### Example

##### SCSS
```
@import 'small';

.message {
  border: 4px solid #ccc;
  padding: 10px;
  color: #333;
}
```
##### CSS
```
h3 {
  font-family: "Source Sans Pro", sans-serif;
  color: #34495e; }
  
.message {
  border: 4px solid #ccc;
  padding: 10px;
  color: #333;
}
```
Note: Importing is beneficial in some situations since you may want a specific scss file to
have attributes of some partial sass files.

## Applying Changes Without `sass input.scss output.css`
You can add changes to your SCSS file and apply them to your css file without having to use 
`sass input.scss output.css` repeatedly. Using `sass --watch input.scss:output.css` allows your CSS
file to get the latest changes from your SCSS file automatically. However only one CSS file can get automatic changes
from a SCSS file. If you want a different CSS file to get new changes from another SCSS file, then you will have to stop 
`sass --watch input.scss:output.css` by using `control + C`

#### Example of Error

SCSS
```SCSS
@import 'small';

.message {
  border: (12px - 2px) solid #ccc;
  padding: 20px;
  color: #333;
}

.success {
  @extend .message;
  border-color:
}
```

CSS
```CSS
/*
Error: Invalid CSS after "  border-color:": expected expression (e.g. 1px, bold), was "}"
        on line 12 of style.scss

7: }
8: 
9: .success {
10:   @extend .message;
11:   border-color: 
12: }
13: 
14: $container-width: 100%;
15: 
16: .container {
17:   width: $container-width;

Backtrace:
style.scss:12
/usr/local/rvm/gems/ruby-2.3.0/gems/sass-3.4.23/lib/sass/entries/parser.rb:1207:in `expected'
```

### Warning
When using `sass --watch input.scss:output.css`, make sure that the changes you made on your SCSS file are correct 
since your CSS file might encounter an error if there is a mistake on your scss file that the CSS file is getting the changes
from.

## Operators

In SCSS files, you can also use operators such as adding and multiplying in order to fix up properties that use px(pixels) or percentages. Operators are
useful as you can use them simultaneously with variables and thus not having to write the same number of pixels repetitively.

### When To Use Operators (side note)
Let's say you want your border to have 30px but you also want your padding to have 5px and your font size to be 10px. Using operators and variables, you first make
a variable that has 30px and then you use it for all other attributes using px. 

#### Example
SCSS
```SCSS
.message {
  border: (12px - 2px) solid #ccc;
  padding: 20px;
  color: #333;
}

$container-width: 100%;

.container {
  width: $container-width;
}

.col-lg-4 {
  width: $container-width / 4;
}
```

CSS
```CSS
.message {
  border: 10px solid #ccc;
  padding: 20px;
  color: #333; }

.container {
  width: 100%; }

.col-lg-4 {
  width: 25%; }
```

## Tips
#### 1. Focus on learning rather than memorizing.
- Tinker and test out lines of code that are most interesting to you or is something you have never seen before. The purpose is to try to understand its functionality on a deeper level. 

#### 2. Comment
- Always comment on every line of code. This is not to make it look nice but to better understand what it does through your own words.
By commenting, you will understand the syntax since your comments/notes proved that you did.

## Resources
- https://www.codecademy.com/learn/learn-sass
- https://www.sitepoint.com/sass-basics-operators/