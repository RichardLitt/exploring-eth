---
layout: post
title: "Licensing an unlicensed repository using script headers"
date: 2018-09-18T22:01:07Z
image: /assets/img/Screen Shot 2018-09-18 at 21.43.51.png
---

While looking around the [@ethereum](https://github.com/ethereum) organization, I noticed that [ethereum/solidity-test-bytecode](https://github.com/ethereum/solidity-test-bytecode) didn't have a license attached to it. This is easy to see on GitHub; even without looking for the existence of a `LICENSE` file, you can check by looking at the listing for the repository in the GitHub organization page. For instance, Aleth here has a license, while our repo does not.

![](assets/img/Screen Shot 2018-09-18 at 21.43.51.png)

You can also check this out in the header for the repository, where a license ought to be flagged to the right of the Contributor count.

![](assets/img/Screen Shot 2018-09-18 at 21.43.41.png)

There wasn't a license for this repository; or much activity at all. That's really not that surprising. The repo is described on GitHub as:

> Test repository for cross-platform comparison of the Solidity compiler

And it is filled mainly with large, semi-inscrutable files. There's no README. There were no issues. And it looks like the history is erased every now and then by the maintainer.

I opened [the first issue](https://github.com/ethereum/solidity-test-bytecode/issues/1), pointing to the lack of a license. Within around two weeks, [@chriseth](https://github.com/chriseth) got back to me, suggesting I add the MIT license I had suggested into the two shell scripts themselves, instead of as an extra file. I hadn't done this before. Just to make sure I knew what I was doing, I looked around on GitHub, and found [this file](https://github.com/OfficeDev/ews-managed-api/pull/30/files) which had an MIT license in a script header. It's the same as adding a `LICENSE` all-caps file in the root directory of a repo, but instead, you simply add the content into the script itself, commented out.

I used [`licenser`](https://www.npmjs.com/package/licenser) to automatically make a copy of the MIT license: `$ licenser print MIT | pbcopy`. Then, I used vim to throw it in the two files, and wrapped the license text itself by setting vim to `:set tw=78` and then using `gq` to automatically wrap the longer two lines. I used a regex to replace my name, which `licenser` had suggested, with `Contributors`, which should work for this repository. After using [`hub`](https://github.com/github/hub) to fork the repo, I committed, pushed to my fork, fetched everything again because sometimes there's a mess-up when using `hub pull-request`, and opened my PR to close the issue I had logged.

Now I'll probably wait a couple of weeks for this to be merged. But, in the meantime, I've learned a couple of things - how to add a license into a script file easily, and why you would do that, and that some @ethereum repos are just dumping grounds for content, as opposed to useful repositories with communities. Does it matter that the only contributor is [@chriseth](https://github.com/chriseth)? No. They've erased the history frequently, so it's possible there were more and GitHub just isn't logging those contributions (which says more about how GitHub logs this, really.)

Good deed done for the day.
