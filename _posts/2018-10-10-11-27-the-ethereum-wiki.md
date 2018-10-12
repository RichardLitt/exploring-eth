---
layout: post
title: "The Ethereum Wiki"
date: 2018-10-10T11:27:39Z
image: /assets/img/logo.png
---

Browsing through the list of repositories, I stumbled upon the [wiki](https://github.com/ethereum/wiki). The repo has over 11k stars, but is fairly spare - there's no documents in the repository, excluding the `.gitignore` and an empty redirect README.

However, the [wiki itself](https://github.com/ethereum/wiki/wiki) is fairly rich. There's a lot to cover, and I skimmed over a lot of the content. At the bottom of the Wiki main page, there's a link to [a proposal to move the Wiki to a Wikipedia-like site](https://github.com/ethereum/wiki/wiki). I think this makes some sense; GitHub's wiki functionality is a bit spare. For most wiki's, I've found discoverability to be an issue, largely because they've been disconnected from the codebase as edits don't reference issues, and because the wiki docs have always been added as an afterthought and quickly became stale. This didn't seem to be an issue here.

One of the issues with the wiki is that it doesn't lend users the same contribution metrics they may get out of making PRs. Contributor activity isn't logged on their profile. However, the tradeoff for maintainers is probably worth it; there's no extra effort needed to maintain issues and to review code.

That isn't always clear to users, though. For instance, [this issue](https://github.com/ethereum/wiki/issues/625) was opened about a spelling error. It took me a few minutes to figure out [where the issue was in the wiki](
https://github.com/ethereum/wiki/wiki/JSON-RPC#returns-31) and to fix it myself. I wonder if this could be sped up, however, by adding content to the README about the point of the repository and how to use wiki's. Right now, that the users know this is taken for granted.

Looking at the issues, I think this is a recurring problem. But the Wiki explictly discourages opening PRs. I want to make the README a bit clearer, and add a GitHub issue template. So, [I asked in the Gitter](https://gitter.im/ethereum/documentation?at=5bc02244ae7be940164194d7). Let's see if James Ray, the maintainer, agrees with me.
