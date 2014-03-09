---
layout: post
title:  "CI Commit Build Hash on Heroku"
date:   2014-01-15 10:52:20
---

We have auto deploys setup on semaphore. Just dropped in the following to our build steps:

```heroku config:set COMMIT_HASH=`git rev-parse $BRANCH_NAME` -a senioradvisor-staging```

```haml
-if !Rails.env.production? && defined? COMMIT_HASH
  %a{href: "https://github.com/SeniorAdvisor/SeniorAdvisor/tree/#{COMMIT_HASH}"}
    #{COMMIT_HASH[0..8]}
```

## Result

[![screenshot of commit hash][commit-hash]][commit-hash]

[commit-hash]: /images/commit-hash.png
