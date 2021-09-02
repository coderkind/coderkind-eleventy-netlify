---
title: "Android Flash player version weirdness"
date: "2010-12-02"
categories: 
  - "adobe-air"
  - "android"
  - "browsers"
  - "flash"
  - "javascript"
  - "web-browsers"
tags: 
  - "android"
  - "flash"
  - "froyo"
  - "version"
---

If I visit [playerversion.com](http://www.playerversion.com) in my HTC Desire Z's Froyo browser it tells me I'm running "FL 10,1,123,425", but when I navigate to Settings > Applications > Manage Applications > All > Adobe Flash Player 10.1 it tells me it's version "10.1.92.10".

I'm still relatively new to Android so this isn't making immediate sense to me; either [playerversion.com](http://www.playerversion.com)'s JS need adjusting or there are two versions of the Flash player on my Android device. Or something else?!?

Edit: [Adobe's own version test](http://www.adobe.com/software/flash/about/) page mirrors [playerversion.com](http://www.playerversion.com)'s findings. [cisnky](http://cisnky.com) suggested trying a pure Flash-based version detection method, which'll be my next move.

Edit 2: [This Flash-based test](http://teppo.tv/kirjoituksia/code.html) mirrors the above; that the minor version I'm running is "123".
