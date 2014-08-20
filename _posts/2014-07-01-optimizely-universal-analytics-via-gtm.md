---
layout: post
title:  "Optimizely & Universal Analytics via GTM"
date:   2014-07-01 11:00:00
<!-- categories: analytics -->
---

# Optimizely & Universal Analytics via GTM

If you’ve done any sort of custom configuration to your Universal Analytics Tag in Google Tag Manager, [@nicholasblexrud’s](https://twitter.com/nicholasblexrud) pattern in “[Add Optimizely with Universal Analytics via Tag Manager](http://www.swellpath.com/2014/04/integrating-optimizely-google-analytics-via-google-tag-manager/)" will leave you - like a ball kicked to Tim Howard - blocked.

Not to fear! Clearhead’s office is streaming the world cup, so we’ve turned off the billable clock and are writing blog posts in between the action. Should be just time enough to photoblog our Optimizely GTM Integration process…

## One Time: GA and GTM Setup
First, we create a series of Custom Dimensions so we can gather data on up to 5 concurrent tests:

![Optimizely and Google Tag Manager Dimensions.png](/images/opt-gtm-dimensions.png)

Next, we create Google Tag Manager macros to look for clearhead.ab1 through clearhead.ab5 variables:

![Optimizely and Google Tag Manager Config.png](/images/opt-gtm-config.png)

![Optimizely and Google Tag Manager Macro.png](/images/opt-gtm-macro.png)

## Yay! We’re all setup.

Every Time: Experiment’s Global JS
Now it’s just a matter of currying the user’s metadata into the global variables via the experiment’s global js (image links to gist).

[![Optimizely and Google Tag Manager Snippet.png](/images/opt-gtm-snippet.png)](https://gist.github.com/tomfuertes/910c8abf4fce40cccfcb)

## That sweet, sweet, data.

![Optimizely and Google Tag Manager Data.png](/images/opt-gtm-data.png)

Obviously lots of moving parts here! If you’re a dev or analyst reading this, we’re hiring and/or hire-able as help!

-Tom

-- xpost from [clearhead.me](http://clearhead.me/post/90510916375/optimizely-universal-analytics-via-gtm)
