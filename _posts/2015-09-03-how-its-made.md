---
layout: post
title:  "How It's Made - Evan's World"
date:   2015-09-03 01:19:00
author: "Evan Markowitz"
---

**Evan's World** wasn't just magically spawned, despite what the lack of git commits when the site was first being built would indicate.  This post hopes to show the design and build process and the sort of decisions that were made.

## Picking my Providers
I was very quick to call up all the companies that helped make this site happen through their services, but the reasons I picked them weren't really brought up.  The idea to bring my site back from the dead started around December of 2014, when I was notified by [GitHub](htps://github.com) about their Student Kit, where they give students (like myself) a bunch of free stuff.

I figured with this I could get my hosting, so I went with [DigitalOcean](https://digitalocean.com) as they gave me a year, and I plan on staying with them in the future once I run out of money.  Besides my **chestnut** server which I am currently hosting with them, I have hosted other small droplets for different projects of mine and I intend on doing so as I need them.

Considering GitHub had hooked me up and I am a huge fan of Open Source, I decided to put all of my source on there as well.  Using Git also meant I can keep track of changes over time and see where I introduced issues.  My site is currently unlicensed though that will change soon, and then anyone could use it to make their own site, like mine.

## Jekyll
I decided early on to use [Jekyll](http://jekyllrb.com) as my site generator as opposed to a platform like WordPress.  This was a very consious decision of mine as it gives me the most freedom with how I run and host my site, as well as allowing further speed increases in the future as I can take easy advantage of CDN's to now not only host my *assets*, but also my content.

## The Server Setup
The server itself is running Debian linux and the web server is nginx.  I used nginx because of its ease of use and speed, as well as the fact that I was more comfortable with it as opposed to Apache.  To deploy my site, I used GitHub webhooks and [jekyll-hook](https://github.com/developmentseed/jekyll-hook) which runs a small server that GitHub pushes updates to, then fetches the updates and builds them again.

## The Theme
The theme was written with [Bootstrap](http://getbootstrap.com) with Creative Tim's [Paper Kit](http://www.creative-tim.com/product/paper-kit) for styling.  I chose Paper because it looked nice, and their Developer License, which all of their "Freebies" are under allows for me to use this theme for my blog and give it away also.  On top of Paper are my own styles to make the site exactly how I wanted it.  I used [Geo Patterns](https://github.com/jasonlong/geo_pattern) to make the randomized patterns in the header images, though currently I am experiencing some issues, which is why all the post patterns look identical.

## Conclusion
Now you've had a closer look at how the site was made, I hope that someone who wants to make their own site can find use in this and take something away from it.  If you enjoy posts like these, many more like this are to come.  If you **don't**, do not worry, I have plenty of other content to come as well.  Until then, see you next time.
