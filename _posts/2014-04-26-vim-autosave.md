---
layout: post
title:  "Vim autosave"
date:   2014-04-26 22:09:44
categories: vim
---

I found myself that I want to autosave in vim. Hopefully after a few googling i summarized with this:
{% highlight vim %}
    set updatetime=1000
    autocmd CursorHoldI,CursorHold * :update
{% endhighlight %}

Put it in your .vimrc and every second of no-doing your current changed buffer will be saved with informational message. 

Just add 'silent!' before ':update' to get rid of the message.

