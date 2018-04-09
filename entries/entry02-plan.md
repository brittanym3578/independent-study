# Entry 2:
## Learning the Basics
<img src = "https://cdn-images-1.medium.com/max/2000/1*lpWLZ75HSCAYYQvx0wxYDQ.png"/>
Photo Credit: https://codeburst.io/how-sass-can-save-you-a-lot-of-time-f1198b658012
## How to install SASS
In order to install SASS into your workspace terminal , you type in `gem install sass`.
If you are unsure whether SASS is installed, type in `sass -v`.
If `sass -v` does not return `Sass 3.4.23 (Selective Steve)`, then SASS is not installed in your
workspace terminal. In case `gem install sass` does not work at all, then try `sudo gem install sass`.

### Creating a Partial File 
A Partial Sass file is a file that has small pieces of SCSS. In order to create a partial sass file, you put an underscore before the name of your file. For example: _partial.scss

## Nesting Properties
In SCSS, selectors are not the only option to nesting, by adding ```:``` after the name of the property can also nest CSS properties.
```
.parent {
  font : {
    family: Roboto, sans-serif;
    size: 12px;
    decoration: none;
  }
}
```
## Saving your SASS file as a CSS file

Once you are done with all of your necessary changes in your SASS file, you can save your changes into
a CSS file by running `sass input.scss output.css` inside of your terminal. Once you did that, you should
see `output.css` in your workspace with all of your changes from your SASS file.

Note: SCSS is another name for a SASS file

## Extend/Inheritance

In SASS, SCSS selectors can inherit other selectors attributes by using `@extend`. `@extend` allows
you to share properties from one selector to another. When a SCSS turns to a CSS file, the selector
that inherits the properties will be shared with other selectors that have similar properties.

#### Example:

##### SCSS
```
.message {
  border: 4px solid #ccc;
  padding: 10px;
  color: #333;
}

.success {
  @extend .message;
  border-color: green;
}
```
##### CSSS
```
.message, .success {
  border: 1px solid #ccc;
  padding: 10px;
  color: #333; }

.success {
  border-color: green; }
```
## Next Steps for week 3 
1. Have a clear idea as to what I will be doing
2. Start drafting my ideas and format it all into an expected result
3. Start watching videos on SASS and learn it on a deeper level
## Tips

#### 1. Workspace is your best friend

- If you want to make sure that your CSS file successfully gets your up to date changes from your SCSS file,
you can put your SCSS file to the left of your workspace and your CSS file to the right of your workspace. That way,
you are able to make sure that your changes are working well on both ends of your files.

#### 2. Take notes while you are studying or practicing on your own

- There will always be a moment when you find something that may be helpful in the near future, but you want to make sure
that you don't forget about it. That is why you should consider taking notes while you are studying as it will be a good 
point of reference in case you want to use something that you learned a while ago. I had to learn this the hard way since I forgot to 
take notes while I was practicing specific lessons. 

#### 3. Codecademy is very helpful
- You are new to all of this, start from the bottom and work your way up. Try the examples and input 
the things you already know. This will help you learn the basics and have a sense of what you will be doing.

## Resources
- https://www.codecademy.com/learn/learn-sass