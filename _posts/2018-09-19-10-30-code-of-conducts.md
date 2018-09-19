---
layout: post
title: "Changing the Code of Conduct for Solidity"
date: 2018-09-18T22:01:07Z
image: /assets/img/logo.png
---

While looking around the [Solidity repository](https://github.com/ethereum/solidity), I saw that @chriseth (whose name I have only just understood as chris+eth - that's certainly an interesting naming scheme) had [recently added a Code of Conduct](https://github.com/ethereum/solidity/issues/4445). The CoC is the standard [Contributor Covenant](https://www.contributor-covenant.org/). You can get a copy easily in your terminal by using [covgen](https://www.npmjs.com/package/covgen), which one of my best friends [@simonv3](https://github.com/simonv3) made, and which I help maintain.

However, if you look at the [Contributing guide](https://solidity.readthedocs.io/en/latest/contributing.html) on Read The Docs for Solidity, the CoC is only mentioned in the Pull Request section. This implies that it doesn't also apply in other spaces: the issues, the Gitter channel, any related Twitter messages, and so on. That isn't how the CoC is supposed to work. The PRs are not the only place where interaction happens.

I proposed a change [in the issue](https://github.com/ethereum/solidity/issues/4445#issuecomment-414875483), suggesting that it should apply to the whole organization. @chriseth pointed out that he doesn't have the ability to enable all of that, but for this repository, it should cover other interactions. Fair.

So, I've made the [following PR](https://github.com/ethereum/solidity/pull/5026) to the ReadTheDocs documentation. The PR template didn't fit exactly, so I deleted some of the checks or wrote that they were `n/a`. But this PR should do the trick.

Now - the question is, who would be in charge enough to know about applying a CoC to the entire organization? I don't think anyone is, at the moment. Something to look into. I've made a [TODO page](TODO) to help me list questions like this in the future.