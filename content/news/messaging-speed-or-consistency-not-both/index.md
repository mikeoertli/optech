---
title: "Messaging: Speed or Consistency, Not Both"
date: "2015-02-03T19:08:33-07:00"
slug: "messaging-speed-or-consistency-not-both"
aliases: ["/news/2015/02/03/messaging-speed-or-consistency-not-both"]
lastmod: "2015-02-12T11:58:54-07:00"
---

Messaging is king, especially text-based messaging. Voice is fine, video has its place too, but there is nothing today that can replace the rapid and highly private aspects of text-based messaging – no headphones required. Given this, it is no surprise that iMessage has been a hit, but other cross-platform apps have been even bigger hits (judging by user count). WhatsApp, Telegram, Hangouts, and others are all trying to be the go-to app for messaging.

This isn't a roundup or definitive review. I want to address the (admittedly first world) problem of getting speed or consistency, but never both. What do I mean by that? Let's take iMessage and compare it to Hangouts for the demonstration, but "Hangouts" could just as easily be replaced with WhatsApp or others.

### iMessage – Brilliant but Inconsistent

When you open iMessage you immediately get your conversation content because it is stored right there on the device. There is no permanent copy on the cloud (<a href="http://techcrunch.com/2014/02/27/apple-explains-exactly-how-secure-imessage-really-is/" target="_blank">details here</a>). Messages are delivered securely to a device and that's the end of it. The result is a lighting fast feel and a negligible launch time, it doesn't even have to ping a server until you send/receive a message or compose a new one (it checks if they're an iMessage user).

Unfortunately, with iMessage you also get inconsistency if you have more than one device with iMessage activated for the account. When my wife sends me a message and she sees it gets "Delivered" she has no idea which of my devices actually got it. You would hope they all did, but that isn't always the case. Technically each iMessage results in the server having N secure and isolated copies where N is the number of devices on your account. Each copy is treated independently and is only removed after it has been confirmed as delivered or it reaches the 7 day expiration. Although this is how it supposedly works, in practice there must be some logic that only confirms a message was delivered to a device and after a certain (very short) period of time it treats all N copies as delivered. Far too many times have I come back to my iPad after a day of missing iMessages on my phone only to find them on my iPad for my assumption to be patently false.

I will stop here and say iMessage usually handles this correctly (far better than it used to), but not always, and not everyone's experience is as good as mine. Messages showing up out of order or some messages never showing up at all are all common problems if you've got more than one device connected to an iMessage account.

### Hangouts – Slow and Steady

Hangouts, on the other hand, never shows messages out of order (or effectively never) and they always show up. Sure you might not get a push notification, but if you open the app they will be there. The main reason behind this is that the master copy of a conversation is on the server, not the device. So if you never get a push notification for a message (which is annoying) the server likely thought you read that message on another device already. This model of having the server as the master means that every time you launch the app it has to ping the server and download updates. Even if you got a push alert with a message, when you launch the app it still pings the server and re-downloads that content that it just showed you in the alert. In iOS you can have a push notification trigger a background download of the message content, but Hangouts doesn't take advantage of this, much to my discontent.

It seems small, perhaps even insignificant, but given with text-based messaging I want to be in and out as fast as my fingers can tap. I will often go in and out of conversations many times in a single minute. Hangouts, despite only requiring a few seconds of my time, feels unusable as an iMessage replacement because of the lag. WhatsApp has similar launch lag and every new message has to be downloaded when the app launches instead of being ready for me when I open the app, unlike iMessage.

Note: I know this launch and usage experience is different on Android, it is far less of an issue there. I still believe iMessage to be a superior experience within the limits it imposes, but it is worth pointing out that these shortcomings are based on the iOS app.

### Solving the Problem

There is a level of complexity to this problem, as simple as it may sound. You don't want to push alerts to 3 devices for every single message if a user is carrying the conversation on one of them. At the same time you don't want to miss message delivery entirely. None of this even matters if the user experience isn't good enough for the messaging app in question to gain the necessary popularity.

How do you solve it? Keep a master copy on a server? Have a "primary" device option? Have behind-the-scenes read receipts? 

I think a combination of fail-safes built on top of the current iMessage strategy is likely he way to go. Avoiding the server-as-the-master solution is the only way to get a truly fast experience. If there were logic to actually check for per-device delivery as well as read receipts  for the server (without having to turn on actual read receipts), most of the issues seen with iMessage today would likely be avoided. It would also make sense to have a primary device either automatically determined based on usage or manually configurable. This could mean that with 100% certainty a single device would always get every message no matter what. There are issues with that device not being connected, but there are solutions beyond the scope of this piece.

### Closing

Text-based messaging is private, convenient, and fast. The private nature makes it intimate and on a personal level makes us trust it and love it in many cases. It is fast, it is reliable (mostly), and it is simple. Anyone can do it regardless of their device or platform; and while we're seeing the proliferation of apps and methods, it has never been more convenient to use text-based messaging to communicate. I believe that the speed and reliability of the experience are key which is why I vastly prefer iMessage to alternatives, the above average level of security helps too. With that being said, I think iMessage has a long way to go for me not to caveat my otherwise emphatic endorsement of it.
