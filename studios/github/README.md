---
title: 'Studio: Github'
currentMenu: studios
---

## Getting Ready: Code Together

Coding together allows you to work as a team so you can build bigger projects, faster.

In this studio, we will practice common git commands necessary when multiple people are developing on the same code base.

## Walkthrough

TODO

## Fireside Story

We are going to play a game. We will play it just like you'd play around a campfire, but on a web page.

Find a new friend to play the game with.

### Player 1

Navigate to your development folder. Follow these instructions to create a new project.

```
$ mkdir fireside-story
$ cd fireside-story
$ git init
```

In that directory, open a new file `index.html` in the editor of your choice. Paste in this code:

```html
<html>
  <body>
    <p>It was a dark and stormy night...</p>
  </body>
</html>
```

Let's check that our html looks allright by opening it in a browser. The URL will look something like this: `file:///Users/cheryl/Development/fireside-story/index.html`.

TODO screenshot

Let's stage and commit this file.

```
$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

    index.html

nothing added to commit but untracked files present (use "git add" to track)
$ git add .
$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

    new file:   index.html

$ git commit -m 'started story'
[master (root-commit) e1c1719] started story
 1 file changed, 5 insertions(+)
  create mode 100644 index.html
$ git log
commit longuniquehashofdigitshere
Author: Cheryl <cherylschaefer@gmail.com>
Date:   Wed Apr 5 10:55:56 2017 -0500

    started story
```


Pick a news site ([The New York Times](https://www.nytimes.com/), for example), and use Chrome Dev Tools to modify one of the main articles to use a picture and text of your choosing. You can have fun with this (see our example below) and take a screenshot to use for a practical joke, if you like.

![Nelly / LC in NYT](lc-nelly-nyt.png)

<aside class="aside-warning" markdown="1">
When linking to an image, pay attention to the protocol -- either `http` or `https` -- of the site you are modifying, and of the image you are including. You can find the protocol at the beginning of the image URL.

If the site you are modifying was loaded over `https` and your image uses `http` then the image may not load properly. You should try to add `s` to the image protocol, and if that doesn't work, look for another image or modify a site that uses `http`.
</aside>

(Optional) Share your creation in the `#fake-news` channel on Slack, and see what others have created!

### Resources

* [Using Chrome Developer Tools: Elements](https://www.youtube.com/watch?v=nV9PLPFTnkE)
* [Chrome DevTools Documentation](https://developers.google.com/web/tools/chrome-devtools/)