---
layout: post
title: My Template
---
> This page is VERY much a work in progress, but sharing the process as it comes along for transparency.

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
- From your [account settings](https://neocities.org/settings) in Neocities, generate an API key for your site by clicking **Manage Site Settings (of target site) > API > Generate API Key**
- [Add the API key as an action secret to your repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template#creating-a-repository-from-a-template) with the name `NEOCITIES_API_TOKEN`

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

1. install [node js](https://nodejs.org/en).
2. navigate to the cloned repository in the [terminal window](https://www.11ty.dev/docs/terminal-window/) 
3. type `npm install` this will install dependencies for the project, and may take a few minute.
4. In the same terminal, start a local webserver by entering `npm start`

You now have a hot-reloading preview of your website! Go 
ahead and start tailoring the template for your comic. When you're ready
 to publish, just [commit](https://docs.github.com/en/desktop/making-changes-in-a-branch/committing-and-reviewing-changes-to-your-project-in-github-desktop) and [push](https://github.com/the-rashons/eleventy-rarebit-template/blob/master) your changes in GitHub Desktop; your site should update on Neocities shortly afterwards!
