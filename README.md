# Risk Enhancements

A mod that adds various enhancements to [Risk: Global Domination](https://www.hasbrorisk.com/).

## Ideas

> This is list of ideas I have collected for this mod. I have roughly ordered them in easiest to hardest to implement, and some may not be possible to implement.

### Easy

- [Fix the slider!](https://www.youtube.com/watch?v=lCSa5nAwq_I)
- Show the ["persona"](https://smgstudio.freshdesk.com/support/solutions/articles/11000077687-our-risk-ai) of bots.
- A better indicator for when a player becomes a bot.
- Add better filters for when searching for lobbies.
- Show player ranks?
- [Other UI/UX improvements?](https://steamcommunity.com/app/1128810/discussions/0/1744521326160244078/#c2259060348518050073)

### Difficult

- Modify placement of blizzards and portals.
- Create and load custom maps.
- More chat emotes.
- A text chat system.
- A replay system.
- A spectate system.
- Create and modify game rules.

### References

- [Discord](https://discord.com/channels/465846009164070912/1020346802236555365)
- [Steam Community](https://steamcommunity.com/app/1128810/discussions/0/1744521326160244078/)

## Notes

> This is my research into Risk: Global Domination. I have not made a significant component of my reverse engineering public yet. At the moment I believe the application is quite exploitable and I don't want my research to be used by malicious actors.

### Overview

[Risk: Global Domination](https://www.hasbrorisk.com/) is developed and published by [SMG Studio](https://www.smgstudio.com/).

- [Amazon](https://gaming.amazon.com/gp/amzn1.adg.product.9e9a8067-b856-4232-89f8-72afad8a0cec)
- [App Store](https://apps.apple.com/us/app/risk-global-domination/id1051334048)
- [Discord](https://discord.com/invite/risk)
- [Facebook Group](https://www.facebook.com/groups/190688308040310/)
- [Facebook](https://www.facebook.com/riskglobaldomination/)
- [Fandom](https://risk-global-domination.fandom.com/wiki/Risk)
- [Forum](https://smgstudio.freshdesk.com/support/discussions)
- [Play Store](https://play.google.com/store/apps/details?id=com.hasbro.riskbigscreen)
- [Reddit](https://www.reddit.com/r/Risk/)
- [Steam Community](https://steamcommunity.com/app/1128810)
- [Steam Store](https://store.steampowered.com/app/1128810/RISK_Global_Domination/)
- [SteamDB](https://steamdb.info/app/1128810/)
- [Wikipedia](<https://en.wikipedia.org/wiki/Risk_(game)>)

The current version of Risk: Global Domination is `3.12.1`. There is a [Android](https://play.google.com/store/apps/details?id=com.hasbro.riskbigscreen), [iOS](https://apps.apple.com/us/app/risk-global-domination/id1051334048) and [Steam](https://store.steampowered.com/app/1128810/RISK_Global_Domination/) version of the application. It was released on Android and iOS in December 2015. The Steam version was released in February 2020.

### Architecture

The application is implemented with [Unity](https://unity.com/). The Unity version used is [`2021.3.16`](https://unity.com/releases/editor/whats-new/2021.3.16). It uses AOT compilation with [IL2CPP](https://docs.unity3d.com/Manual/IL2CPP.html).

The developers have published the [dice logic on GitHub](https://github.com/smgstudio/risk-dice). It has not been updated since 2021 and was for version `3.3.0`.

At least from [this Q&A with the developers](https://www.youtube.com/watch?v=VqFy4u03x6Q) the current game uses a peer-to-peer networking. The developers are in the process of updating the game to use a client-server networking, which should be released soon.

Accounts can be [reported and banned](https://smgstudio.freshdesk.com/support/discussions/topics/11000017727). In addition the game does have a cheat detection built-in...
