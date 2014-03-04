---
layout: post
title:  "Google/Universal Analytics and Rails"
date:   2013-12-24 10:52:20
<!-- categories: analytics -->
---

## Quick Post

If you're using Google Analytics or Universal Analytics, you should send the
`contoller` and `action`. It lets you do some pretty crazy report pivoting
without having to teach everyone regular expressions.

## Google Analytics

{% gist tomfuertes/65ab92733d5de3fc042c ga.js %}

[![screenshot of page types in Google Analytics][ga]][ga]

## Universal Analytics

{% gist tomfuertes/65ab92733d5de3fc042c analytics.js %}

[![screenshot of page types in Google Analytics][ua]][ua]

[ga]: /images/ga-custom-var-page-type.png
[ua]: /images/ua-custom-var-page-type.png
