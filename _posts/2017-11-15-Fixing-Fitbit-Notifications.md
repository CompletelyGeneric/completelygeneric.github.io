---
layout: post
title: "Fixing Fitbit Notifications"
feature-img: "img/pale_feature_image.png"
---

I recently purchased a Fitbit Ionic smartwatch, and, after having useful notifications removed from my Charge 2 in an update, I purchased it knowing that notifications were, for all intents and purposes, broken on Android.  
So I wrote an Xposed module to make them actually useful. If you're interested in that,   
[here's a gist](https://gist.github.com/CompletelyGeneric/3418a3a555fab5192b39b7111e6f242a) (I'll put everything in a proper git repo and upload it to the Xposed repo soon). If you want to hear a rant about bad UX, keep reading.  
  
Currently, notifications on fitbit devices "respect" Android's Do-Not-Disturb feature - meaning that if you've set your phone to DND, you won't get notifications. This boggles the mind. If I have my phone on me, and set to vibrate or ring; I probably don't need my fitbit to vibrate as well. And worse, If I have my phone set on DND, my watch will not receive notifications.  
The most infuriating part of this is that all Fitbit devices (that i've owned at least), have device specific DND features that you can set independently from the phone.   

I can only imagine that this decision was motivated by complaints of people who were woken up at night by notifications; Which is an understandable motivation. What isn't though, is the decision to not give the user an option to override their phone's DND settings.

I really like my Ionic, but I'd really like an official fix to this.