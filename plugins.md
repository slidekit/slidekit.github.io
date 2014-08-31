---
layout: default
title: S6 Format for Plugins / Addons
---

# {{ page.title }}

## Custom Events 

S6 fires the following events (to let plugins/addons get hooks into the JavaScript machinery):

* `slideshow.init`
* `slideshow.start`
* `slideshow.keys( key )`
* `slideshow.debug.on`
* `slideshow.debug.off`
* `slideshow.change( from, to )`



{% include questions.md %}
