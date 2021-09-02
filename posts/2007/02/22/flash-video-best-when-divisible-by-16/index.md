---
title: "Flash video best when divisible by 16?"
date: "2007-02-22"
categories: 
  - "flash"
  - "flex"
  - "video"
---

I've been looking into whether better-quality Flash video is produced when sticking to dimensions that are divisible by 16. This seemingly has been the rule with older codecs, but I've had to investigate the issue for Flash 8 .flv video. Adobe [doesn't seem to think so](http://www.adobe.com/devnet/flash/articles/encoding_video_print.html), stating:

> Although these ratios are standard, and should be used to avoid distorting the video, the size of the encoded video is not set in stone. The original web video sizes used heights and widths that were evenly divisible by 16. This was mandatory for many early codecs. Although this is not necessary for modern codecs, you should stick to even heights and widths.

This doesn't quite tally with the advice on [On2's site](http://www.on2.com/support-resources/flix-tutorials/flashvideoquality/) (producers of the Flash 8 codec):

> If you reduce your video size (image dimensions), your picture will be sharper. Another small factor you may consider is that optimal frame sizes are divisible by 8. That means that if your image dimensions (width and height) are divisible by 8, you will be wasting as few bits as possible on encoding data for portions of the video which do not actually appear. This is a complex issue relating to the way image compression uses 16x16 and 8x8 blocks to form an image.

A forum post by Zappu [here](http://videocharge.com/forum/index.php?t=msg&goto=464&S=42d398f2290db0518f0610495b92d917) enforces the 16/8 rule, as does this entry on [MultimediaWiki](http://wiki.multimedia.cx/index.php?title=On2_VP6). Conversations with Dave Curtis (hello Dave!) have been very helpful and also seem pretty conclusive on the "16 issue".

It's probably best to stick to dimensions divisible by 16, but not set in stone. Complex clips with lots of motion and/or panning would probably benefit from the 16-rule to a greater extent. I hope to produce some encoded tests myself, but if anyone has any in the meantime the links would be much appreciated.

Why is there so little clear information on this on the web?!?
