---
title: "Adobe Live 2007"
date: "2007-06-21"
categories: 
  - "accessibility"
  - "adobe-air"
  - "flash"
  - "flex"
  - "javascript"
  - "video"
---

Adobe Live was a two-day event held in Angel on the 5th-6th June which showcased a number of new technologies on offer from Adobe, along with various seminars and talks from industry professionals.

Below are the rough notes I took (more of a brain dump, but I haven't the time to format it right now).

### Flash

- Flash 9 at 84% as of March this year
- Flex 3 will allow greater control over skinning/creative aspects
- Check out [http://www.picnik.com](http://www.picnik.com) for a Flex-based online image editor
- Video encoder not packaged with normal Flash; have to buy CS3 package or professional version it seems
- Top5 mobile phone makers signed up to put Flash on their medium/high end phones
- Flash Lite 3 announced
- Adobe Device Central is database and emulator of mobile devices running Flash. Very impressive. Can calibrate performance of machine to the performance of the device you're previewing for. Aiming to update device support list every quarter.
- In Flash CS3, Quicktime export and video importing improved
- Can deinterlace video when importing
- Fullscreen and caption buttons now in video skins
- 3D won't import into Flash from Photoshop; will be a 2D render of the last frame
- Title and Description metadata now part of the .swf you publish from Flash
- Adobe Media Player allows you to skin your player/channel according to how you want (I think it runs off RSS)
- Apparently, when it comes to the interactive aspects of AMP you'll need Flash Media Server (i.e bringing on an ad, overlay, dynamic ad playlists, etc)
- AMP does bandwidth detection
- Adobe are thinking about IPTV, but can't announce anything
- ABC, Desparate Housewives, etc run their video online via FMS
- [http://www.videojug.com](http://www.videojug.com) is a progressive download site
- Encrypted streams coming later in the year (dunno if through AMP or not)
- Flash Media Server runs off Windows, and will remain Windows for a good time. Priority is to add features for the product rather than add cross-platform support
- Photoshop (PSD) import works with older PSDs regarding retaining layers; don't need a CS3 PSD to enjoy this functionality

### Mobile Platforms

- Focus on mobile interfaces is that space is at a premium; don't have a weather button that loads a new page that gives you loads of options – have that initial weather button immediately bring up general weather information and have futher weather options underneath. Every click/page should be providing some essential information; make the steps between information as few as possible
- iPhone realises that menus for different phone apps (e.g. images, mp3 player, etc) shouldn't be generic; you want to perform different tasks/things in each section, so the menu should tailor specifically for what the application's trying to achieve. Doesn't always make sense to have generic menus on all applications
- Check out Flash Cast; doesn't seem to use the mobile browser. MTV use it a lot to push their rich visual-based content
- Mobile content can't be a port from the desktop; need to specifically target mobile users
- Mobile development isn't generic; you need to look at the performance, input methods and screen size of the mobile device you're planning on targeting
- On the low-end devices you can still bring in dynamic data, so on those lower devices you can present the same data but with fewer animations, etc

### Apollo

- In the past, applications based firmly in the browser, mainly Windows-based
- Check out [http://www.finetune.com](http://www.finetune.com). Can't just listen to a song; need to hear it as part of a playlist. All content is being licenced, so legit site
- Finetune Flex application has iTunes integration, so it can look in your iTunes library and suggest different playlists based on what music you already have
- Apollo has recently added local database support, so seemingly mirroring Google Gears
- Apollo can use ActionScript, Flex, XML, Video, Audio, HTML, PDF, JavaScript, CSS and SQL
- Plan is for Adobe and Google to form a common API for use in Gears and Apollo, but at early state of discussions
- Both Gears and Apollo use SQLite
- Apollo APIs are NOT available to ActionScript 1 or 2
- Scout – Apollo-based HTML/JS debugger
- Apollo uses WebKit Open Source Engine (same as Safari, KHTML), because it's open source, small filesize, proven, and also offers mobile support
- SQLite works as a file basically; you say where you want the SQL file, and then all API calls are made to that file. Single install, easy
- Apollo Functionalty – Network Detection, File I/O, Custom Window Chrome, Multi-Window, Native Menus, Drag n Drop, Clipboard access, System Tray and Dock Notifications, Application/Installer Signing, Application Icons, File Type Registrations, Background applications, Application Update APIs, Supports XML-RPC, SOAP, Rest-Based Web Services, Binary and Web Socket support
- If you want to build an application with deep hardware integration, then probably go with something like C++, .NET, etc. However, Adobe believe there is a gap between browser-based applications and those hardcore hardware-based applications; this is where Apollo fits in
- Much lower learning curve to building applications in Apollo, as most the skills are known by web developers
- Workflow – Develop/debug in IDE or command line, package application for deployment, distribute application package
- Apollo requires a runtime install, and then for each application a specific application install
- Looking into getting Apollo runtime install fed in via Flash install in the future possibly
- Apollo runtime is about 5-7MB install
- .air files are the Apollo application extensions, and they'll work cross-platform
- Hoping to have runtime and application files available as downloads, so when distributing content you can package in the runtime too

### Flash/Flex working together

- Fireworks CS3 has Flex components built-in which you can export at the same time as you export your image. You select “export images and MXML” option
- Main advantage of this is that a designer can create a layout/design which you can export from Fireworks and use as the starting blocks for your Flex application (you can choose the generated MXML file as being the main file for the new Flex Project you've created)
- Two ways a designer can produce assets within Flash that can be used by a coder; export the timeline as MXML, and COMMANDS > MAKE FLEX COMPONENT. This extention is available within Adobe Labs right now. Exports it as a .swc file. HAS to be a movieClip in order to export it. Within Flex you then update your library path to point to the location where you've exported your .swc and then Flex can use the new component.FLEX BUILD PATH > LIBRARY PATH (via right-clicking top directory within your project layout panel)
- You add a namespace for your local generated components from Flash, and then Flex can use your components the same as any other, with all the properties exposed via code hints
- Can export from Illustration .swfs that can then be used as skins for Flex components
- Flex 3; better for designers – easier to import assets, will be able to skin easier
- Flex 3 Beta to be released very soon
- Fireworks is the only graphics application that features Flex components and also allows you to export directly to MXML
- When you export for Flex, it HAS to be 25FPS, as that's the default framerate for Flex applications. There are other caveats too apparently, but the feature is still in Beta, so expect changes and increased functionality when finalised
- If you export something with more than one frame from Flash and a Flex component, then those different frames will be treated as different “states” within Flex

### RIA Development

- Adobe dealing with the Spry framework for AJAX
- Spry is fairly design-centered
- 1.4 is current release, with 1.5 currently on Adobe Labs
- Distributed on an Open Source Licence
- Find the effects demo of Spry's stuff (looks like [script.aculo.us](http://script.aculo.us/))
- Looks good for form validation (ticks, date checkers, etc)
- Dreamweaver CS3 supports Spry (Spry widgets, effects and data sources)
- Spry looks to be clean code-wise; it adds class names to DIVs
- Can use data binding to bring in stuff according to the data source
- Lots of demos and sample code in with Spry
- Flex/Flash allows you to push information to the browser, rather than polling the server
- Look for the flipbook medical demo; looked excellent!!!
- FABridge is used to communicate between Flex and AJAX
- Kristophe Konrad Flex's SQLAdmin for Gears demo – look it up
- Nice demo using Flex to extend Google Maps; used Flex to allow user to scroll map and have another user see where he's scrolling, can see other person via webcam, can draw on map and other person see it in real-time, etc
- LifeCycle Data Services; enables real-time pushing of data from/to AJAX or Flex clients
- Fresh is an Apollo application built using the Yahoo! Model for AJAX (doesn't use Flex or Flash)

### Flex 3

- Flex 3 applications will still target Flash 9 player
- Both Apollo and Flex 3 will be available this year
- Able to extend Flex builder (Eclipse) easier, so you can add your own extensions, etc
- Because Flex 3's SDK is open source, Flex builder will be able to support multiple SDKs, so you can choose which SDK you want to publish with
- Flex 3 supposedly better regarding localisation and accessibility
- Advanced datagrid in Flex 3; can sort on multiple columns at the same time, not just one
- Can format individual cells (assign cells their own styles)
