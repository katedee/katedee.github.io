---
layout: post
title: Tools + Account Setup
---

Let’s get some account making and tools-instaling out of the way! I will also briefly explain what each of these does (over-simplifying in some cases, but we don’t need the nitty gritty of it). All the accounts and tools I recommend are completely free, or in one case, have a generous free plan. 

Don't worry about doing anything other than installation yet. We will walk through things together later on ☺️. If this feels overwhelming, that's ok! You don't need to remember these definitions, I just offer them because I know they can be helpful.

## Github Account

From [wikipedia](https://en.wikipedia.org/wiki/GitHub){:target="_blank"} “GitHub is a proprietary developer platform that allows developers to create, store, manage, and share their code.” So basically it’s a website that stores our code and on it you can create repositories that (for our purpose) will host the code that makes up your site, and, as you make changes, keep a sort of “archive” of previous versions of the site. This is handy because should we ever do something massively wrong, we can either rollback the changes, or dig up older versions of certain files.

To begin, [create an account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github){:target="_blank"}.

> **If your comic features adult content**: Github is a bit wishy-washy with their [adult content policies](https://docs.github.com/en/site-policy/acceptable-use-policies/github-sexually-obscene-content){:target="_blank"}. I would recommend "privating" your repo which will make incredibly unlikely your repo gets flagged (I see _public_ NSFW repos exist on git all the time so it seems they aren't actively looking, let alone private repos which would require that somehow someone knows AND they have a paid account which lets them reach github to report it). BUT, if that's still a concern, you can just host your images on [one of these free image hosts](https://www.reddit.com/r/imguralternatives/comments/12vk0i0/comparing_the_nsfw_imgur_alternatives/) that allow NSFW content. The instructions for the rest of this template will remain the same--you'll just post a url for your images, but I will outline that in the necessary spot ✨
{:class="warning"}

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
One of these will serve as your "host" and at a certain points, instructions will diverge a bit (these will be noted).

For now, here's a comparison of the two:

| Feature | Netlify | Neocities |
|---|---|---|
| Adult content is okay | ✅ | ✅ (but hit the 18+ checkbox) |
| Generous free plan | ✅ [100GB bandwidth](https://www.netlify.com/pricing/){:target="_blank"} | ✅ [200GB bandwidth](https://neocities.org/supporter){:target="_blank"}, admittedly larger than Netlify, though in either case you're unlikely to hit the limit. |
| Allows custom domains | ✅ | ❌ only on supporter plan |
| Cross Origin Support (like getting a file from google sheets, which is what we will need to later add a comments section) | ✅ | ❌ only on supporter plan |
| Social aspect of a user-site directory | ❌ | ✅ |
| Create multiple sites | ✅ | ❌ only on supporter plan |
{:class="plan-comparison"}

For the record, I don't inherently think one is better than the other. It comes down to a matter of preference. Neocities will cost you more than Netlify, but supporting Neocities is a pretty worthwhile cause.

The instructions going forward will assume you're proceeding with Netlify. If you're not using Netlify, ignore those bits, and I will provide neocities specific instructions where necessary.

Whichever one you choose, create an account for it. For going with Netlify, you can create an account by using your Github account in sign up :).

- [Netlify](https://www.netlify.com/){:target="_blank"}
- [Neocities](https://neocities.org/){:target="_blank"}

