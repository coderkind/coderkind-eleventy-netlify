---
title: "How to debug IE7 silent crashes"
date: "2011-10-03"
categories: 
  - "browsers"
  - "javascript"
  - "web-development"
tags: 
  - "ie"
  - "ie7"
  - "internet-explorer"
---

Experiencing a problem where a page randomly crashes in Internet Explorer 7 with no warning.

Work-in-progress blog posting, but found this so far: [http://groups.google.com/group/IEToolbar-Group-Bugs/msg/fd808abaa72524ea?pli=1](http://groups.google.com/group/IEToolbar-Group-Bugs/msg/fd808abaa72524ea?pli=1).

The crash report requires more Googling it seems:

Access violation - code c0000005 (first chance) eax=00000000 ebx=00000001 ecx=00000000 edx=00000007 esi=00219ec8 edi=00000000 eip=3cf6e923 esp=01e5ddf0 ebp=01e5ddf0 iopl=0         nv up ei pl nz ac pe cy cs=001b  ss=0023  ds=0023  es=0023  fs=003b  gs=0000             efl=00210213 \*\*\* ERROR: Symbol file could not be found.  Defaulted to export symbols for C:\\W INNT\\system32\\mshtml.dll - mshtml!DllGetClassObject+bfa45: 3cf6e923 8b490c           mov     ecx,\[ecx+0xc\]     ds:0023:0000000c=???????? 0:005>
