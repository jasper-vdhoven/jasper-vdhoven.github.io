---
layout: category-post
title:  "Game Launcher UX - Comparing bandwidth restriction options"
date:   2022-05-31
categories: Games UX
---

# Introduction

With games pushed more and more onto digital stores, an increasing amount of people are forced to use these varying launchers to download their games. And as is well known, not everyone gets the same internet connection. This lead me to wondering how the various game launchers handle restricting the bandwidth that they can use for their downloads.

This article will go into how the launchers from Valve, Good old Games (GOG from hereon out), EA, Epic Games, Ubisoft, Rockstar, and Activision Blizzard handle the restricting of available bandwidth. A comparison will be made based on whether the individual launchers support this and what options the launchers give the user in relation to bandwidth restrictions.

# Steam - best case

First up is the Steam launcher made by Valve. Steam is the largest of the launchers covered here in terms of users, it has also been around for the longest amount of time and seen many iterations.

Looking back through some older Steam versions, the ability to add a bandwidth restriction has existed since about 2013 listed in [this ghacks][ghacks-steam] article. The Steam client shown featured a dropdown menu listing various speed presets, starting at 128 Kbps up until 250 Mbps:

![Steam client circa 2013 showing download bandwidth restriction options](/images/Games/Launchers/Steam-general-download-options-2013.webp)

Furthermore, you could select the connection type that you had and its approximate available bandwidth.

In the current Steam client (2022-05-20) the options are a bit more expanded while also more restricted. The new client depicted down below now shows a text field where the end user can enter a custom value. The value entered within this box will limit the speed to that amount in KB/s, rather than using a series of presets. This change to me is a welcoming change as this allows for better fine tuning than a preset can offer for varying internet connections.

One thing that needs to be looked after is whether the option to "Display download rates in bits per second" is set as this has an impact on the bandwidth limit set in the options. The first image shows a configuration in MB/s with the second in Mb/s:

![Steam client in 2022 showing download bandwidth restriction options in MB/s](/images/Games/Launchers/Steam-general-download-options-2022-MBs.webp)

![Steam client in 2022 showing download bandwidth restriction options in Mb/s](/images/Games/Launchers/Steam-general-download-options-2022-Mbps.webp)

Setting a bandwidth limit of 120 MB/s is about 960 Mb/s, or a gigabit connection, 8 times the amount of the Mb/s filter.

The option to specify the connection type and an approximate speed have been removed, which whilst maybe unfortunate is not horrible to me. The speed approximate is not needed if the user can set the best value by themselves.

Over all, the Steam client is the launcher I have used to most. But I also think it offers the best settings for bandwidth restrictions as it no longer relies on prefixes and allows the user to set the value themselves.

# GOG Galaxy

Up next is the launcher made by GOG named Galaxy and acts as a competitor for Steam, offering DRM-free versions of popular and older titles. The company behind the launcher is Polish studio CD Project Red, famous for The Witcher and Cyberpunk 2077. Besides the sale of DRM-free games, the major selling point of Galaxy is that it can connect to other services, including Steam and act as a global hub for all your games.

The Galaxy launcher has existed since 2019 in closed beta and released to the general public on December 18, 2019 as 2.0.12 Beta. The current version of Galaxy is 2.0.50.34 Beta and offers support for bandwidth limitations:

![GOG Galaxy client circa 2022 showing download bandwidth restriction options](/images/Games/Launchers/GOG-Galaxy-bandwidth-limitations-2022.webp)

Similar to Steam, Galaxy allows the user to set the bandwidth limit themselves in either MB/s or KB/s; no option for Mbps or Kbps is present which is a bit saddening but better than only presets or not being able to set a limit at all.

# Origin

Origin is a launcher that I have never really enjoyed using since my first introduction to it with Battlefield 3, many years ago. The UI was always clunky with items not where I expected them; something that has persisted over time it seems.

Origin has support for download bandwidth limits since circa 2017, after the community had been asking for it for years on their [EA Answers HQ][ea-answers-hq] page. The thread this community post is referring to contained the following hilarious conversation between a _passionate player_ and a (retired) community manager:

![EA Answers HQ discussion regarding the implementation of download bandwidth restrictions](/images/Games/Launchers/EA-answers-download-restrictions.webp)

Since the 2017 release EA Origin does support limiting the amount of bandwidth to be used by downloads, albeit only with presets outside and during gaming. The options given are quite disappointing to me, only going from 16 KB/s up to 50 MB/s or 400 Mb/s.

![EA Origin showing the different options available for download restrictions outside gameplay](/images/Games/Launchers/Origin-download-bandwidth-limit-2022-out.webp)

Moreover, the only way to disable downloads whilst playing a game is via the dropdown and selecting "Don't download during gameplay":

![EA Origin showing the different options available for download restrictions during gameplay](/images/Games/Launchers/Origin-download-bandwidth-limit-2022-during.webp)

Allowing the end-user to set the bandwidth limit would be a better alternative than any preset could offer, but considering it took EA 4 years to implement this I would say that's more than most would have expected in the first place.

# Ubisoft Connect

Up next is Uplay, now branded as Connect, and is Ubisoft's take on Origin for their own games. However, unlike EA, Ubisoft publishes (most of) their games on Steam as well, and then forces you to use Connect alongside Steam rather than only Connect.

Looking back through the years it appears that Uplay/Connect has been able to set a bandwidth limit since 2016, going by [this][yt-ubi-dlbandwidth] YouTube video showcasing the available options. The mechanism shown in the video is the exact same as the one that is present now in Connect. This mechanism is sadly a **slider** that ranges between 0.25 MB/s and 200 MB/s, or 1600 Mb/s, which is a tad bit excessive in my opinion for **most** connections:

![Ubisoft Connect download bandwidth restriction options](/images/Games/Launchers/Ubisoft-Connect-download-settings.webp)

My issue with this slider design is that, whilst it has a wide range of options, it doesn't feel intuitive to use. In my situation with a 180 Mbps connection I would use at most ~22% of the slider. Moreover, setting the value is a nightmarish experience on its own as the set value only updates once the user let's go of the slider to set its position. Individual, smaller adjustments are in 0.25 MB/s increments up and down.

![Ubisoft Connect download bandwidth restriction slider behaviour](/images/Games/Launchers/Ubisoft-Connect-bandwidth-slider-behaviour.gif)

It was this terrible design that even led me to writing a short collection of Tweets regarding the slider, and my discontent with it, that would ultimately get turned into this article:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">.<a href="https://twitter.com/UbisoftSupport?ref_src=twsrc%5Etfw">@UbisoftSupport</a> Is there a reason to have the download bandwidth limiter set to Megabytes per second, rather than Mega- or kilobits per second?<br><br>The current scale ranges from 0.25 MB/s to 200MB/s; this is 2 mbps and ~1600 mbps respectively.</p>&mdash; Jasper (@Saszper) <a href="https://twitter.com/Saszper/status/1520853998235967488">May 1, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

# Rockstar Games

Rockstar's launcher is by far the most useless out of the bunch, as was made clear yet again with the release of the GTA Trilogy Definitive Edition where the release of this new game the launcher failed to inform people about news regarding the launch and current release date of a title. The topic is covered in detail by Australian YouTuber DarkViperAU in a video titled: [The FAILURE Of The Rockstar Games Launcher and GTA Trilogy Definitive Edition Launch][yt-dvau-gta-trilogy]; beware, the video has strong language!

To my surprise, the launcher does support the limiting of bandwidth for downloads. However, this is only via presets between 128 KB/s up to 100 MB/s or 800 Mb/s:

![Rockstar Games download bandwidth restriction options](/images/Games/Launchers/Rockstar-Games-download-bandwidth-restrictions.webp)

# Epic Games Launcher

One launcher I had forgotten about was the Epic Games one as I have used it sporadically. To my surprise, however, within its limited settings menu there was an option to limit the download speed for game downloads. To my even bigger surprise, not a slider or preset menu, but a value the user could enter in KB/s instead!

![Epic Games Launcher and its download throttling options](/images/Games/Launchers/Epic-Games-Download-Throttling.png)

This small addition places it above the likes of major game publishers stuck on presets or a half-assed slider. But all is not great, as it appears that the feature had been in the oven on the community forum since **April 7, 2015** only shipped in 2020 as can be seen in [this][reddit-eg-client] Reddit thread. Over on the community forum the comments are less hilarious as those from EA, but sad nonetheless over the amount of time required to get this implemented:

![Epic Games forum with upset community members](/images/Games/Launchers/Epic-Games-Forums-upset-community-members-over-lack-of-throttling.png)

![Epic Games forum with mentioning the now shipped features](/images/Games/Launchers/Epic-Games-Community-Forum-throttling-finally-shipped.png)

> [Epic Games Forums][eg-forum] thread in question.

# Activision Blizzard Battle.net

Last, but not least, Activision Blizzard's Battle.net launcher for their own games that has been around for forever.

The Battle.net has support for bandwidth restrictions for downloads that are entered by the user in a text box with measurements in KB/s and nothing else. This came as a surprise to me, not expecting Activision Blizzard to actually offer this in a way that was not a set of presets. It is however, a bit saddening that they don't show a conversion to MB/s or Mb/s to help users better understand the values they have entered as their connection is most likely measured in MB/s or Mb/s nowadays.

![Activision Blizzard download bandwidth restriction options](/images/Games/Launchers/Activision-Blizzard-Battlenet-launcher-download-bandwidth-restrictions.webp)

After a bit of digging it turns out that this functionality has existed until at least 2017 as can be seen in [this][yt-activision-blizzard] YouTube video tutorial. In the worst case scenario that this is only added in 2017, Activision Blizzard have managed to implement it better than most of the other launchers in the space that were created **after** Battle.net even.

# Conclusion

All in all, all the launchers that were tested have supported the limiting of download bandwidth with some better than others.

The worst offender in my opinion is still Ubisoft's Connect with its horrible slider design that scales in increments of 0.25 MB/s and slider that only updates when you let go of it. This design is worse than the presets offered by Origin and Rockstar as those at least give users a setting that will be in the range of where they want it be with minimal effort. In contrast, Ubisoft Connect requires more effort as the slider lacks any markings for values and can only change in steps of 0.25 MB/s. I sincerely hope that Ubisoft will change this design in the (near) future and make it usable, rather than **un**usable.

As for the remaining launchers, I compiled a short table with each launcher and how they handle it for quick reference: 

| Launcher name | Bandwidth limits supported? | Options on offer? |
| ----------- | ----------- | ----------- |
| Valve - Steam | ✅ | User entered values in either Mb/s or MB/s |
| GOG - Galaxy | ✅ | User entered values in either KB/s or MB/s |
| EA - Origin | ✅ | Presets ranging between 16 KB/s and 50 MB/s |
| Epic Games - Launcher| ✅ | User entered values in KB/s |
| Ubisoft - Connect | ✅ | Slider with values between 0.25 MB/s and 200 MB/s |
| Rockstar Games | ✅ | Presets ranging between 128 KB/s and 100 MB/s |
| Activision Blizzard - Battle.net | ✅ | User entered values in KB/s |


[ghacks-steam]:                         https://www.ghacks.net/2013/04/24/steam-client-beta-update-brings-long-awaited-download-speed-limiter/
[ea-answers-hq]:                        https://answers.ea.com/t5/Origin-Client-Web-Technical/How-do-I-set-maximum-download-speed-in-origin/td-p/1444230
[yt-ubi-dlbandwidth]:                   https://youtu.be/j7Q1Wfr9r_0
[yt-dvau-gta-trilogy]:                  https://www.youtube.com/watch?v=DO0YQLhxzRw
[reddit-eg-client]:                     https://www.reddit.com/r/EpicGamesPC/comments/gaf7yb/egs_feature_update_you_can_now_able_to_throttle/
[eg-forum]:                             https://forums.unrealengine.com/t/limit-launchers-download-speed/26719
[yt-activision-blizzard]:               https://www.youtube.com/watch?v=_nBH02xL_Ns