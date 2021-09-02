---
title: "Preventing string break-out from container"
date: "2012-08-15"
categories: 
  - "web-development"
---

Useful tip outlined on [Smashing Magazine by Chris Coyier](http://coding.smashingmagazine.com/2012/08/13/coding-qa-with-chris-coyier-responsive-sprites-responsive-font-sizing-media-query-efficiency-more/) on preventing text from breaking out of containers.

> .prevent-text-breakouts {
>   -ms-word-break: break-all;
>       word-break: break-all;
>       word-break: break-word;
>   -webkit-hyphens: auto;
>      -moz-hyphens: auto;
>           hyphens: auto;
> }
