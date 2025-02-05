---
layout: post
title: First Changes
---
We're going to dip our toes into some code touching, by dealing with the required parts of the starter message of our template.

## Metadata
> 1. Update _data/metadata.js with your webcomic info, and author info. This is important for generating your RSS feed.

Open up vscode, and on the main window drag and drop the entire project folder (TODO SCREENSHOT). In the left sidebar you should see a list of your files now. Locate the `metadata.json` file (in the _data folder) and click it to open it up in vscode. You should see something like this:
(TODO SCREENSHOT)

> TIP: you can also open files in vscode by hitting cmd+P or ctrl+P and start typing the filename. It should pop up in the list of suggestions and you can choose it from there
{:class="tip"}

Fill this out with your comic info, making sure you keep what you type between quotation marks as seen in the file. For the `base` field, you will enter what will end up being your final url for your website. For example `https://example.com` if you are going to setup a custom domain, or your netlify/neocities url  (`https://your-netlify-url.netlify.app/` or `https://your-neocities-url.neocities.org`).

Save the file once changes are done.

## Delete the starter message
> 2. Delete this message from _includes/layouts/base.liquid.

Continuing in VSCode, open up the `base.liquid` file (`_includes/layouts/base.liquid`). Delete lines 38-61 (or for those not in vscode, the entire bit between `<!-- Delete this message -->` and `<!-- Stop deleting -->`). Save the file.

If you ended up doing the step to have a hot reloading site, and have a server going, you should see this change in your browser. If not, no worries, you should see it later.

## A summary of the rest of the message

## A couple last things...
While we're doing more broad layout/site edits, let's update the comic banner image ("Your Logo Here"), and the favicon if you wish (optional, but it's the little explosion emoji in the tab).

### Logo/Banner image
If your comic doesn't have a banner image ready yet, that's okay. You can either choose to skip this bit, or grab a random image to use for now and follow along.

The `logo.png` image is located in the `img` folder. There are two ways of dealing with updating it:

**If you don't wanna code touch:** Create a banner image, that is at least 500px wide (use empty space in the iamge if you want a smaller logo), and save under the same name and file extension, writing over `logo.png`.

**If you're game for some more learning (it's not too bad, promise):** 
- place the image you'd like to use for your banner in the `img` folder. 
- in vscode, open the `header.liquid` file (using the cmd+P/ctrl+P trick or locating the file under `_includes/header.liquid`). On line 6, you'll see that we're linking the banner image there. Change `logo.png` to the name of your image, keeping in mind the code is _case sensitive_ (so `logo.png` and `Logo.png` are two completely different files according to code. Similarly `jpg` and `jpeg` are not the same to the machine). Write any alt text for the image between the quotation marks of the `alt=""` attribute.

### Favicon
The favicon image is also found in the `img` folder. Follow similar steps as above for the favicon image, choosing to either override the image with the exact same name and file extension (`favicon.png`).

If you want to take the chance to swap it yourself, exactly as before, place your favicon image in the `img` folder and then update the details of it in the file (it is found in `base.liquid` which we were in before, on line 17). If you change the file extension, be sure to reflect that in the `type` attribute. So if you use a `.jpg` file, change `type="image/png"` to `type="image/jpg"`.

## Commit and push
Whew, that was a lot of changes!

Before moving forward, let's get a little more familiar with Github desktop. Now that you've done some changes, you should see on the left of Github Desktop a list of changed files. To the right, it will show the differences (in red the things you delted, in green what you added)

TODO SCREENSHOT

We're going to now save our changes, and push them back up to the repo online, which will trigger a deploy/build and update our site online.

First look in the bottom left of Github Desktop. You'll see in the corner two fields "Summary of Changes" and "description". For summary of changes, you'll put in a title that encapsulates the changes we made. Description will be a more detailed couple sentences or list of what you've done. It is optional, but I recommend it as it will help you refer to things, if you ever need to go back and refer to what changes you made when.

So for example, you might fill out this commit like so:

```
summary: 
Updated site metadata and images

description: 
Filled out info in metadata.json
Deleted starter message in base.liquid
Updated banner image and favicon
```

Once that's done, hit the `commit to main` button.
On netlify, you should see a site deploy was triggered (make sure you're on your site dashboard, and then choose `deploys` from the left). You can follow along as it builds, or wait for it to finish. Once done, you can hit that `view production deploy` button again, or go to your site link.

For neocities, wait a few minutes and you should see your changes.

> SOMETHING WENT WRONG! If your build failed on Netlify, or you're not seeing the changes on neocities, go back over the instructions and make sure you have the correct file names in place (remember, case sensitive!), or that you didn't accidentally delete a quotation mark (or a comma in metadata.json)


TODO check how the site handles smaller banner images, adjust css accordingly

 
