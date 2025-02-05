---
layout: post
title: Fork, Deploy, Clone
---

Here is the first instance which our paths diverge between Netlify and Neocities. I will begin with Netlify instructions.

## Fork & Deploy

### Netlify
If you're going to host on Netlify, to fork and set up the repo to Netlify, click this button: 

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/katedee/eleventy-webcomic)

You will get an e-mail from Github about an SSH key being issued, don't worry, that's part of it. It's a thing that allows Netlify access to the code on github.

Once you hit the button, it will deploy to Netlify and you can watch as it builds. Once it's read, you can click "Open production deploy" and see it yourself! If you'd like to change the random generated name before `.netlify.app`, you can do so by clicking "site configuration", and under "site information", hit the "change site name" button.

### Neocities
1. Go to [my template repo](https://github.com/katedee/eleventy-webcomic){:target="blank"}, and hit the fork button along the top right. 
2. From your [account settings](https://neocities.org/settings){:target="_blank"} in Neocities, generate an API key for your site by clicking **Manage Site Settings (of target site) > API > Generate API Key**
3. [Add the API key as an action secret to your repository](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions#creating-secrets-for-a-repository){:target="_blank"} with the name `NEOCITIES_API_TOKEN`

## Back together 
Okay, now open up github desktop, which we downloaded earlier. Click the "clone a repository from the internet". If you've clicked away from this screen, no worries, you can find the same option under "File" in the top menu. From the selection list, you should see the repo you just created/cloned, select it and clone it, choosing a convenient location on your computer to reach.

## Local Setup (optional)
> Note: this bit is very much optional, so feel free to skip. I offer it here because we're most of the way there for this and it offers some nice benefits, but you'll be okay without it. You can always come back later and try this for future site editing, so no pressure right now.
{:class="note"}

Local setup?! Local setup let's you have a hot-reloading (hot-reloaing basically means it refreshes the site as we make changes, so you see them right away) version of the website through your command line/on your computer to preview your changes before you push them up to your repository.

This part requires using the `Terminal` app on your computer, but don't worry, I'll guide you through everything and it's not going to horribly mess things up.

1. install [node js](https://nodejs.org/en){:target="_blank"}.
2. navigate to the cloned repository in the [terminal window](https://www.11ty.dev/docs/terminal-window/){:target="_blank"}. You can do this by typing `cd path/to/your/repo`, where `path/to/your/repo` is the series of folders you dive through to get there, for me for example, I type `cd documents/code/eleventy-webcomic`
3. type `npm install` this will install dependencies for the project, and may take a few minute.
4. In the same terminal, start a local webserver by entering `npm run start`, it will spit out a bunch of things, and, assuming no errors, end in something like
`Server at http://localhost:8080/`, open a browser tab and go to the localhost link it spits out.

You now have a hot-reloading preview of your website! This is nice because you can preview changes locally, before pushing them up to your repo and deploying to netlify/neocities. Sometimes between changes you'll need to refresh the page, but mostly it handles it.

When you're done with doing changes and no longer need the local server running, go to the terminal window, and hit ctrl + c to stop the server.

TO DO: link to dev tips, terminal basics tutorial maybe.





 
