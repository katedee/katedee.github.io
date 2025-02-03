---
layout: post
title: My Template
---
> This page is VERY much a work in progress, but sharing the process as it comes along for transparency.
{:class="warning"}

* TOC
{:toc}

# Getting Started

Hello there! Thanks for choosing my template, and diving into setup with me. This guide seems intimidatingly long, but that’s because I am trying to make it thorough with the idea that you have little to no prior coding experience.

If you’re new to code, I know it seems spooky, but I promise you it’s going to be alright! I once was scare of code too, and panicked any time I got a blank screen or something went wrong. Now I understand it is just a puzzle that needs to be solved— and one that you are encouraged to take breaks from as necessary. Nearly nothing you do can’t be undone if needed, and I will try to guide you through this as smoothly as possible.

**TIP :** There is this belief amongst the non-coding public, and sadly even among some snooty developers, that people who code are special or better-than. They are not. I had a friend once says that “coders are just like plumbers— we just happen to know where to bang on the pipes”. They too once made plenty of mistakes like we will (and probably still do!).

## Tools + Account setup

Let’s get some account making and tools-instaling out of the way! I will also briefly explain what each of these does (over-simplifying in some cases, but we don’t need the nitty gritty of it). All the accounts and tools I recommend are completely free, or in one case, have a generous free plan. 

Don't worry about doing anything other than installation yet. We will walk through things together later on ☺️. If this feels overwhelming, that's ok! You don't need to remember these definitions, I just offer them because I know they can be helpful.

### Github Account

From [wikipedia](https://en.wikipedia.org/wiki/GitHub){:target="_blank"} “GitHub is a proprietary developer platform that allows developers to create, store, manage, and share their code.” So basically it’s a website that stores our code and on it you can create repositories that (for our purpose) will host the code that makes up your site, and, as you make changes, keep a sort of “archive” of previous versions of the site. This is handy because should we ever do something massively wrong, we can either rollback the changes, or dig up older versions of certain files.

To begin, [create an account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github){:target="_blank"}.

### Github desktop

Great! Now that you’ve got an account, we’re doing to download github desktop. It will also install the latest version of git for us (GIT is the thing that actually allows you to manage and track your code, github is the site that allows us to share that online—over simplified, but sufficient).

This tool will let us “pull” down the code from the online repository, keep track of changes we make to it locally (like adding images, or comic posts, etc), and then “commit” those changes where we write a message about what we’ve changed, and then “push” those changes back up to our online repository. This is the thing that helps us keep almost archives of our site, should we ever need it.

[Grab the installer here!](https://github.com/apps/desktop){:target="_blank"}

### VS Code (optional, but strongly recommended)
[Visual Studio Code/VS Code](https://code.visualstudio.com/){:target="_blank"} is a free code editor. I mark this as optional, because ultimately you could use something like TextEdit on mac, or NotePad on windows, but VS Code is miles better because it colour-codes parts of your code. My screenshots later one will be from within VS Code so it might also be helpful for following along.

But just to illustrate the point, here's what a file looks like on TextEdit vs VS Code.

<figure>
    <img src="/img/code_editors.png"
         alt="TextEdit vs VS Code">
    <figcaption>There are more benefits to VS Code, but the colour coding, and line numbers will probably be the biggest helps to us.</figcaption>
</figure>

#### Liquid Syntax Highlighter (optional)
So the "colour coding" I talk about is called Syntax Highlighting, if you wanna get all technical. This is optional, but will be helpful and the install is straightforward. Open up VS Code, hit `CMD + Shift + P`, and type `install extensions`, hit the first suggested result of "install extensions". You'll then see some things pop up in the sidebar. In the searchbar there, type "liquid". The first result is what we need, hit the blue install button (not seen in screenshot because I already have it).

### Netlify or Neocities account

---

## TO WRITE ABOUT

- setting the base url in settings
- talk about setting things in metadata.json
- mention the home page and strip being pretty similar

### Setting up accounts (And what it do)

- Github
- Netlify or Neocities

## once repo is set up
- with netlify there’s not much to do, other than to begin editing in github
    - maybe naming the site on netlify?
    - custom domain stuff
- neocities instructions (these are from the rashons repo, I have not personally tested this workflow)
- From your [account settings](https://neocities.org/settings){:target="_blank"} in Neocities, generate an API key for your site by clicking **Manage Site Settings (of target site) > API > Generate API Key**
- [Add the API key as an action secret to your repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template#creating-a-repository-from-a-template){:target="_blank"} with the name `NEOCITIES_API_TOKEN`

## Editing files using github / making changes

- [ ]  FOR INITIAL SETTING UP, RECOMMEND GITHUB DESKTOP + VS CODE
    - [ ]  look at you being a coder ✨
- [ ]  mention github history and how to see that on a per-file basis
- [ ]  mention keeping track of your changes
- [ ]  mention how to see commits which will show all files changed for a particular commit
- [ ]  site structure (where comic images go, where other images go, where comic posts go)
- [ ]  go over starter message stuff, and then delete it (mention how to find it in history, or reference on my site)
- [ ]  swapping logo
- [ ]  writing a comic post (note that things are CASE SENSITIVE, and jpeg is not the same as jpg)
    - [ ]  markdown cheat sheet
    - [ ]  edit my existing posts (as warm up)
    - [ ]  write about in the future how to do this on the github website if in a pinch
- [ ]  the archive
- [ ]  changing arrow buttons
- [ ]  swapping favicon
- [ ]  emoji keyboard shortcut
- [ ]  OH NO! SOMETHING’S GONE WRONG!
    - [ ]  take a deep breath, it’s going to be okay.
    - [ ]  remember that github saves past versions of our site, and netlify only deploys if something isn’t absolutely breaking.
    - [ ]  review our last commit. What did we change?
    - [ ]  is the file extension correct? the filename (remember, case sensitive!)

## Netlify Deploys

- [ ]  write about where to find deploys
- [ ]  write about what failed means
- [ ]  opening console maybe?

## For Local Development

### Tools to download:

- github desktop
- vs code (optional, but strong recommended)
    - after vs code install: liquid syntax package
- node js

TO DO: write about local development and why

1. install [node js](https://nodejs.org/en){:target="_blank"}.
2. navigate to the cloned repository in the [terminal window](https://www.11ty.dev/docs/terminal-window/){:target="_blank"} 
3. type `npm install` this will install dependencies for the project, and may take a few minute.
4. In the same terminal, start a local webserver by entering `npm start`

You now have a hot-reloading preview of your website! Go 
ahead and start tailoring the template for your comic. When you're ready
 to publish, just [commit](https://docs.github.com/en/desktop/making-changes-in-a-branch/committing-and-reviewing-changes-to-your-project-in-github-desktop){:target="_blank"} and [push](https://github.com/the-rashons/eleventy-rarebit-template/blob/master){:target="_blank"} your changes in GitHub Desktop; your site should update on Neocities shortly afterwards!

 
