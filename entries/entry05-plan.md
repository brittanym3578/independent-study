# Entry 5:
## Implementation
<img src = "https://media.giphy.com/media/FUQQ3WPJZEULe/giphy.gif"/>
Photo Credit: https://giphy.com/gifs/inside-out-gif-FUQQ3WPJZEULe
## Check In 
I have recently been trying to form ideas on what to build on my website and how to implement what I have learned into the website I have in mind.
I went back to some of the basics I have learned before and tried to incorporate it with other forms of code to see how they work together.

### How functions Work in SASS

When making a function in your SCSS file, you need to define the name and what it's placeholder variable name is. Example:`@function set-notification-text-color($color)` 
Then you set the conditionals and what you want the function to do when your code meets the function's if statement or not. Note: If and else should look like this, `@if` and `@else`.
When your SCSS file gets transferred over to a CSS file, your function will not show up since CSS does not recognize what a function is.

Function example:

SCSS
``` SCSS
@function set-notification-text-color($color) { //name of function, what variable it grabs, $color = placeholder name
  @if (lightness($color) > 50) {
    @return #000000; // If background color is light, return dark to $color
  } @else {
    @return #ffffff; // Else, return light color to $color
  }
}

```

### After taking a closer look at the code below, 

```Sass
sass --watch input.scss:output.css
```

I realized that two files are part of that command, `input.scss` and "output.css". So, 
I went ahead and created those using the touch command. Then I ran the new command I found out about, 
```Sass
sass input.scss output.css
```

## What is the “--watch” command ?

Actually, the “--watch” command is not a “command”. It’s called a flag.
The “--watch” flag tells Sass to “pay attention” to the folders /scss and /css, so when you make changes to
the .scss file (demo-styles.scss) Sass will detect the change and compile the SCSS file into the final CSS file you’re going
to use on your website or app.
All tutorials I’ve read make you watch specific files, like this:

```sass
sass --watch styles.scss:styles.css
```

## Next week Goals
* Start add more sass code to get css code for my website.
* To start finding some information on what my website is going contain, or one of my previously made websites to incorporate sass to it.

### <strong>Takeaways</strong>
- When taking notes put things in your own words, if you were to copy word for word you would not be able to actually understand what you're learning
- **Don't try to do too much.** Understand your own limits and go build from there. This refers back to Mr.Mueller's MVP where you have to start from the simplest project first and slowly build upon that project to have more and more functions. You can not start building a house with a roof. You have to start with the basics, the foundation.
- I find the best way to organize my thoughts and accomplish goals efficiently is to <b>make to do lists</b>