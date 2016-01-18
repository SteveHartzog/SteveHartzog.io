---
layout: post
title:  "Web Apps have finally arrived"
date:   2016-01-07 22:00:55
description: This is a sample description.
categories:
- guides
banner_image: web-apps.png
comments: true
---
So What is a web app? Well, it's a web application of course. But a web app is so much more than a URL running in Chrome.

In order to be a web app it must have the following characteristics:

1. An app with a *custom icon*, distinctly ***separate*** *application icon*, not just a tab in Chrome.
1. An app that does not have the normal chrome address line or bookmarks bar.
1. An app with it's own separate memory space.
1. An app that shows up as distinctly different when you alt-tab.
1. And, at least on Ubuntu, an app that you can launch by searching via Unity (like Windows Run).

But I had to figure out how to do it. It was a long journey, but I did it. 

### Here are the steps to take on Ubuntu 15.10 (Unity):

1. Go to the site that you want to make an application, and in the Chrome menu bar select:
**File | Create application shortcuts...**
1. Find an application icon and save it to **~/.local/share/WebAppIcons**.
1. Add this icon to the shortcut by editing the shortcut properties and drag and drop a good icon (128x128 or 256x256 for HiDPI)
1. Move the shortcut to **~/local/share/applications**.
1. Optionally drag to the launcher.

### Here are the steps to take on Mac OS X (El Capitan):

1. Download an application icon and save it to **~/WebAppIcons**.
1. Using the [fluidapp](http://fluidapp.com), set the URL, and select the icon you saved earlier at ~/WebAppIcons. This will create the shortcut and place it in your /Applications folder.
1. Drag and drop the app to your dock.

> **Note**: There are other ways to do it in OS X, but they are all significantly more complex... and I just wanted to create a quick app!

### What's good?
Here is a small sample of the ones I use.

* **Evernote Web** (yea, who knew that Evernote didn't have a linux version... and, no, Everpad is not a viable replacement IMHO)
* **Google Plus**
* **Gmail**
* **Google Calendar**
* **Google Play Music**
* **Google Sheets**
* **Google Docs**
* **Google Slides**
* **OneNote Online** (meh, it works)
* **Outlook Online** (for my corp mail)
* **Pocket**
* **Feedly**
* **Jira** (I have one app per project)
* **Confluence**
