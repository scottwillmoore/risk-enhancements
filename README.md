# Risk Enhancements

A mod that adds various enhancements to [_Risk: Global Domination_](https://www.hasbrorisk.com/).

## Ideas

> This is list of ideas I have collected for this mod. I have roughly ordered them in easiest to hardest to implement.

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

> This is my research into _Risk: Global Domination_. I have not made a significant component of my reverse engineering public yet.

### Overview

[_Risk: Global Domination_](https://www.hasbrorisk.com/) is developed and published by [SMG Studio](https://www.smgstudio.com/).

- [Amazon](https://gaming.amazon.com/gp/amzn1.adg.product.9e9a8067-b856-4232-89f8-72afad8a0cec)
- [App Store](https://apps.apple.com/us/app/risk-global-domination/id1051334048)
- [Discord](https://discord.com/invite/risk)
- [Forum](https://smgstudio.freshdesk.com/support/discussions)
- [Play Store](https://play.google.com/store/apps/details?id=com.hasbro.riskbigscreen)
- [Reddit](https://www.reddit.com/r/Risk/)
- [Steam Community](https://steamcommunity.com/app/1128810)
- [Steam Store](https://store.steampowered.com/app/1128810/RISK_Global_Domination/)
- [SteamDB](https://steamdb.info/app/1128810/)
- [Wikipedia](<https://en.wikipedia.org/wiki/Risk_(game)>)

The current version of \_Risk: Global Domination is `3.12.1`. There is a [Android](https://play.google.com/store/apps/details?id=com.hasbro.riskbigscreen), [iOS](https://apps.apple.com/us/app/risk-global-domination/id1051334048) and [Steam](https://store.steampowered.com/app/1128810/RISK_Global_Domination/) version of the application.

### Implementation

The application is implemented with [Unity](https://unity.com/). The Unity version used is [`2021.3.16`](https://unity.com/releases/editor/whats-new/2021.3.16). It uses AOT compilation with [IL2CPP](https://docs.unity3d.com/Manual/IL2CPP.html).

The developers have published the [dice logic on GitHub](https://github.com/smgstudio/risk-dice). It has not been updated since 2021 and was for version `3.3.0`.
