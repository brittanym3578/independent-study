# Entry 6:
## Starting with the Project 
<img src = "http://i.imgur.com/7C0ws9e.gif"/>
Photo Credit: http://www.hilariousgifs.com/working-with-css/

## Planning 
After completing Codecademy and trying out different things based on SASS, I have began to form ideas for my desired website.

My first thought was that I knew that instead of just making a website with just information, I wanted to make something that could possibly be helpful to me or other people.

## Am I using CSS or SASS?
- At first I was really confused with the way my code looked because it looked like regular CSS but then I realized that in my cloud9, my code automatically changes into SASS.
[Example](../images/img-2.png)

```Sass
sass --watch input.scss:output.css
```

I realized that two files are part of that command, `input.scss` and "output.css". So, 
I went ahead and created those using the touch command. Then I ran the new command, 
```Sass
sass input.scss output.css
```

Upon doing that, I realized that a file with the name `output.css.map` was created, and it contained specific code as the image in the example above

I was happy with the result but what was it for ?
- I realized that this is finally how SASS could easily work:
    - After making two files, one input, and output; All you have to do is type your 
 (SASS) code in the input file, then SASS does all the work and transfers the worked up
code to the `Output` as a regular css file your HTML could understand.


### Last thing: <br>
You could use the 

```Sass
sass --watch input.scss:output.css
```
After you get your input and output files set up. 
What that does is tell Sass  to watch the file and update the CSS every time the Sass file changes.
Yes, that would happen regardless, when you type into input save, and refresh. However, that command saves you from all the hassle and
makes life easier by allowing you to see real-time changes to your `output.css` file as you type 
into your `index.scss` file. It's actually pretty cool to see too!

## Confused and Lost 
- How do I link my html template to my SCSS ?
    - [Example](../images/img-3.png)
    - Of course, I believe that you can link your code to your Sass using 
```Html
<link rel="stylesheet" href="output.css">
```

- Can I still use CSS ? 

## Next week Goals
* Start add more sass code to get css code for my website.
* To start finding some information on what my website is going contain

### <strong>Takeaways</strong>
1) Look back at your notes. When you start working on your project you begin to feel overwhelmed with what you have learned in the past few weeks. It is okay to forget some things, that is why we made entries.
2) Start Googling. Never be afraid to look up specific things you need in order to move on with your project or feel like you have not gone through it thoroughly. 
3) **Ask your classmates for help.** We are all working on a project and some may be working on the same topic as you. Share ideas, share your obstacles, learn from one another.