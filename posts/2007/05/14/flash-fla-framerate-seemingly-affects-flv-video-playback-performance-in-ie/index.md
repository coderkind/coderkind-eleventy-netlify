---
title: "Flash .fla framerate seemingly affects .flv video playback performance in IE"
date: "2007-05-14"
categories: 
  - "flash"
  - "video"
---

I've been doing some work using the FLVPlayback component to make a generic video player application, but noticed recently that video playback performance was choppy within Internet Explorer (6 and 7) compared to Firefox.

After a quick search I found [this forum post](http://www.kirupa.com/forum/archive/index.php/t-228942.html), and after changing the framerate of my .fla from 12fps to 24fps I found performance within IE to be comparable to Firefox again.

I hate these "it shouldn't be the case, but is" rules with Flash sometimes.
