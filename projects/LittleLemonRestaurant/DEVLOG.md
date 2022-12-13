## About This Project
This project is part of the lessons from Meta's HTML and CSS in depth course. I'm just creating this project to follow along the course lessons.

## LOGBOOK
Tue 13 Dec 00:57:19 +08 2022
As I started this project, I want to practice some git workflows and get comfortable with the terminal. 

This project, as will other projects, lives on a separate branch. I created a new branch by `git branch <new-branch-name>` and switched to it with `git checkout <new-branch-name>`. I will continue working here with the usual `git add` and `git commit` commands. And subsequently, I will be publishing this local branch in the remote repository with `git push -u origin <new-branch-name>`. 

Tue 13 Dec 01:10:58 +08 2022
At this point of writing, I'm at "Video: Semantic tags in action". The video lesson is simply the instructor writing out the HTML structure for `blog.html`. 

Whilst following the lesson, I realised that typing the HTML tags in Neovim feels like a chore. There has to be some way to make the typing process more efficient. This is something worth investigating as manually typing the HTML tags as I did seems to leave room for errors. 

I also realised that it might not be a good idea to use a different editor than the instructor. After completing the code, the instrutor used Live Preview from within VS Code. I'm not sure how I could do the same with my current setup.

Tue 13 Dec 01:23:43 +08 2022
I've learnt how to achieve the same thing as VS Code's Live Preview in the command-line. Install [live-server](https://www.npmjs.com/package/live-server) globally with `npm install -g live-server`. Then run `live-server` in the project directory and voila! To stop the server, `CTRL+C`. Hopefully, this is enough for me to follow along with the rest of the course without complication.

Speaking of complication, I may have written the `blog.html` file. But I don't have any of the other files used in the lesson. I don't have the `styles.css` nor do I have the `logo.png`. So while I may have been able to fire up a server and preview my `blog.html` file, it won't look the same as the instructor's preview. Am I missing something here? I'm pretty sure they didn't ask me to download any files prior to this lesson. Oh wells, whatever.


Tue 13 Dec 01:33:57 +08 2022
An alternative to installing `live-server` is to use `python3 -m http.server`. I'm not sure if `live-server` offers more features but this alternative method wouldn't require any installation, I think. The article [How do you set up a local testing server?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server) has more details.  


Tue 13 Dec 01:47:10 +08 2022
As someone who's not a stranger to HTMl, I'm quite surprised to learn of [The Description List element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl). It's used to enclose a list of groups of terms and descriptions.

```html
<dl>
    <dt>Term</dt>
    <dd>Description</dd>

    <dt>Another term</dt>
    <dd>Description</dd>
</dl>
```




Tue 13 Dec 20:18:57 +08 2022
Some vim tips; 

`o`/`O` adds new line and switch to insert mode, below/above the current line.

`w` moves the cursor to the the start of the next word.
`W` moves the cursor to the start of the next WORD.
`e` moves the cursor forward to the end of a word.
`E` moves the cursot forward to the end of a WORD.
`b` moves the cursor to the start of the previous word.

`{`/`}` move the cursor to the previous/next paragraph

`f<character>` moves the cursor to the next occurence of <character>
    eg. `f{` moves the cursor to the next occurence of `{`.


`zz` center the cursor on the screen


`cw` change (replace) to the end of the word
`ciw`/`ciW` change entire word/WORD
`cit` change all the content in a HTML tag. **USEFUL FOR EDITING HTML TAGS**

