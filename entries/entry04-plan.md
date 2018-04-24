# Entry 4:
## Starting a Plan
<img src = "https://www.elegantthemes.com/blog/wp-content/uploads/2014/06/Using-Sass-with-WordPress.jpg"/>
Photo Credit: https://www.elegantthemes.com/blog/tips-tricks/how-to-use-sass-with-wordpress-a-step-by-step-guide

## How do functions function?

In SASS, you use a function by determining what color aspect do you want to change such as `saturate()` or `darken()`. After that, you add the hex color code
(Personally, I prefer using variable as it keeps track of the hex code) and the amount of color that you want to change in percentage. There are some functions
that do not require a percentage. When the file is carried over to CSS, the function will change into a hex code.

### Example
Note: Notice the hex code number

SCSS
```SCSS
.darkness{
  $boxcolor: #9276e0;
  background: darken($boxcolor, 30%);
}
```
CSS
```CSS
.darkness {
  background: #42239a; }
```

#### Darken() and Lighten()
The darken function makes a color darker while the lighten function does the opposite.

#### Saturate() and Desaturate()
The saturate function makes a color more saturate and the desaturate function makes color
dull

## Compass

Compass is an add on to SASS that allows you to organize your SCSS and CSS files in separate folders and, keep track of changes from a specific SCSS file to CSS
When I was using Compass to start creating my app, I spent less time trying to find a file since everything was organized clearly and I was able to look at my changes from 
my CSS file.

### How to install Compass

Before you install compass in your workspace, you first need to install SASS and cd to your project folder. After that, use `gem install compass`. Once you install compass, you will 
get two folders in your project folder. One folder has SCSS files and the other folder has CSS files.

[Example](../images/img-1.png)

### Getting the latest changes from SCSS using Compass
You need to cd into your new CSS folder if you want a CSS file to get the latest changes. When you are in your CSS folder, use `compass watch example.css` to track any SCSS file of the same name 
to give changes to the CSS file.

### Trying Inheritance Once Again 
The only way you use inheritance is by the @extend feature, that, in fact, is, what inheritance is. The @extend feature. Okay, what exactly is the _@extend_ feature?
@extend is a feature of Sass that allows classes to share a set of properties with one another. Selectors that @extend a class in Sass will have their selector included right up next to the class it is extending, resulting in a comma separated list.

Its syntax looks like this:
```Sass
@extend .class-name;

```

Examples of Usage: <br>
```Sass
.foo {
  color: black;
  border: 1px solid black;
}

.bar {
  @extend .foo;
  background-color: red;
}
```
```Sass
This is compiled to:

.foo, .bar {
  color: black;
  border: 1px solid black;
}

.bar {
  background-color: red;
}
```
In the example above, .foo and .bar are defined which have the following features:

.bar inherits from .foo, containing all properties of parent class .foo.
.bar extends .foo by adding the property background-color.
### Plan 
I'm making a website in which I will use HTML to code and incorporate SASS in it to test my understanding of it.
This is the last week I will be practicing the basics and now I'm ready to move onto the drafting of my project.
### <strong>Takeaways</strong>
<ul>
<li>I found it helpful to try to <b>break ideas down</b> in order to better understand them, as well as, to try and <b>visualize</b> them or utilize <b>images and diagrams</b> to increase comprehension</li>

<li><b>Explore</b> different learning methods and try to <b>find what works for you</b> or what type of learner you are</li>

<li><b>Simplicity.</b> If you get your code to work how you want, find ways to improve. It is not only beneficial for you to make sure the concepts being taught are well grasped by you, but it also prevents long tedious code. Also, by making the code easier, it gives you more working room . In the beginning , i was using several lines just to get the music to appear. Now, we can add effects and breaks using looping.</li>
</ul>
