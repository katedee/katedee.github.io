---
layout: post
title: Tools + Account Setup
---
> This page is VERY much a work in progress, but sharing the process as it comes along for transparency.
{:class="warning"}

* TOC
{:toc}

Let’s get some account making and tools-instaling out of the way! I will also briefly explain what each of these does (over-simplifying in some cases, but we don’t need the nitty gritty of it). All the accounts and tools I recommend are completely free, or in one case, have a generous free plan. 

Don't worry about doing anything other than installation yet. We will walk through things together later on ☺️. If this feels overwhelming, that's ok! You don't need to remember these definitions, I just offer them because I know they can be helpful.

## Github Account

From [wikipedia](https://en.wikipedia.org/wiki/GitHub){:target="_blank"} “GitHub is a proprietary developer platform that allows developers to create, store, manage, and share their code.” So basically it’s a website that stores our code and on it you can create repositories that (for our purpose) will host the code that makes up your site, and, as you make changes, keep a sort of “archive” of previous versions of the site. This is handy because should we ever do something massively wrong, we can either rollback the changes, or dig up older versions of certain files.

To begin, [create an account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github){:target="_blank"}.

## Github desktop

Great! Now that you’ve got an account, we’re doing to download github desktop. It will also install the latest version of git for us (GIT is the thing that actually allows you to manage and track your code, github is the site that allows us to share that online—over simplified, but sufficient).

This tool will let us “pull” down the code from the online repository, keep track of changes we make to it locally (like adding images, or comic posts, etc), and then “commit” those changes where we write a message about what we’ve changed, and then “push” those changes back up to our online repository. This is the thing that helps us keep almost archives of our site, should we ever need it.

[Grab the installer here!](https://github.com/apps/desktop){:target="_blank"}

## VS Code (optional, but strongly recommended)
[Visual Studio Code/VS Code](https://code.visualstudio.com/){:target="_blank"} is a free code editor. I mark this as optional, because ultimately you could use something like TextEdit on mac, or NotePad on windows, but VS Code is miles better because it colour-codes parts of your code. My screenshots later one will be from within VS Code so it might also be helpful for following along.

But just to illustrate the point, here's what a file looks like on TextEdit vs VS Code.

<figure>
    <img src="/img/code_editors.png"
         alt="TextEdit vs VS Code">
    <figcaption>There are more benefits to VS Code, but the colour coding, and line numbers will probably be the biggest helps to us.</figcaption>
</figure>

### Liquid Syntax Highlighter (optional)
So the "colour coding" I talk about is called Syntax Highlighting, if you wanna get all technical. This is optional, but will be helpful and the install is straightforward. Open up VS Code, hit `CMD + Shift + P`, and type `install extensions`, hit the first suggested result of "install extensions". You'll then see some things pop up in the sidebar. In the searchbar there, type "liquid". The first result is what we need, hit the blue install button (not seen in screenshot because I already have it).

## Netlify or Neocities account

