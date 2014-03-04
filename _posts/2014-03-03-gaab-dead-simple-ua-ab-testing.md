---
layout: post
title:  "gaab - Universal Analytics AB Testing"
date:   2014-03-03 10:52:20
<!-- categories: analytics -->
---

# [`gaab`][repo] - Dead Simple Universal Analytics AB Testing

[`gaab`][repo] is a microlib I started for @FUWeekend. Attending Howard Abrams talk at
[jQueryCon Portland][jqcon-portland] was eye opening. I followed along only to
look around and see others eyes glaze over when he started talking about GUIDs,
hashing keys, bucketing, etc... AB Testing can and should be much more simple.
`gaab`'s code is [< 45 lines][code] as of 0.2.0 and abstracts AB Testing into
what I hope is a super approachable api.

```javascript
gaab('jumbotron', 1, [
  { variation: 'control' },
  { variation: 'spiffy', 'h1': 'Spiffy :)' },
  { variation: 'boring', 'h1': 'Boring :(' }
]);
```

[![screenshot of gaab][gaab-example]][gaab-example]

[![screenshot of reporting example][gaab-reporting]][gaab-reporting]

[Go forth and test][repo]

[jqcon-portland]: https://www.youtube.com/watch?v=FZ1ROac50J0
[gaab-example]: /images/gaab-example.gif
[gaab-reporting]: /images/gaab-reporting.gif
[code]: https://github.com/tomfuertes/gaab/blob/master/lib/gaab.js
[repo]: https://github.com/tomfuertes/gaab
