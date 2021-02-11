---
author: Luis
date: 2018-10-18 06:07:00
header-img: img/in-post/luis-paul-junior.jpg
subtitle: Careful! Loudnorm does more than just change the volume!
categories:
  - Audio
tags:
  - DIY
  - Music
  - Audio
title: Why FFmpeg Loudness & Normalization Guides Are All Wrong, Evil & Immoral!
url: /2018/10/18/audio_norm_guides_are_evil_and_immoral/
ShowReadingTime: true
---


## The Wrong Way
There are SEVERAL guides online telling you how to normalize audio to provide a great listening experience by using FFmpeg’s "loudnorm" filter. Most walk you through a simple process called "track normalization." You set a goal loudness, and adjust every piece of audio up or down to match that loudness. This is evil and immoral and I’ll tell you why:

Loudnorm changes the way things sound!

Loudnorm crushes dynamics!

## The Right Way
The right way™ is "Album Normalization," where every piece of audio (song, level soundtrack, etc.) gets normalized in relation to the loudest piece of audio.

> "With album normalization, just the loudest tracks of an album are made equally loud and the other tracks keep the relative level they had on their album." - Eelco Grimm, loudness researcher


## Why You Need Good Audio/Loudness Normalization
If you’re a developer creating a VR experience, or a game, or something where music features heavily, you need to do normalization, and you need to do it right.

You can’t just normalize every piece of audio to a certain average level and call it good.

Not normalizing audio = poor user experience

There can still be jarring sound transitions. You ever watch TV at a comfy volume, realize the show is going to commercials, and feel dread flood through your body, ears recoiling in fear because you know the commercials you’re about to see will be 10x as loud as the show?

Yeah, good normalization fixes that.

So unless you want your users to hate you, normalize your audio properly!

Now what happens if you normalize your audio wrong, crushing the dynamic range?

Honestly, a lot of people probably won’t even notice (circa 2018).

But once good normalization becomes the standard for all experiences including audio, people WILL hear the difference between a great normalization algorithm and the loudnorm kludge copy-pasted from Stack Overflow, and they will HATE it. And don’t you want your users to have the BEST experience?

## The Proof of Why People Love Good Normalization

"Alright tough guy," you say, "what makes you so qualified to talk about audio like this?"

Well, I’m really not. I have very little ethos here. But I’m STILL positive users love properly normalized audio.

Why?
Cause TIDAL hired a smart guy, with a ton of audio street cred, to do a study on best normalization practices. He sent non-normalized & normalized versions of a playlist to 38 people. And guess what?
80% of people preferred the album normalized versions to track normalized! (Link to study) [https://octo.hku.nl/octo/repository/getfile?id=qLlZPGSVXFM]. And those 80%, 9% said they’d never accept track normalization (an inferior normalizing method) if it were turned on by default!

Ok, I admit at least one of subjects was an audio nerd, as Ian Shepherd (legendary mastering engineer) admits he was a part of the study in his (great post on the subject)[http://productionadvice.co.uk/tidal-normalization-upgrade/]. Regardless, 31/38 people is a pretty strong majority. I imagine the study would translate well to a larger sample of non audio nerds as well.

## In Conclusion...

Be careful following guides online dealing with subjects you’re not familiar with. It can be tempting to just do what Google’s Loudness page says, without realizing they’re giving recommendations for Google Assistant developers. It can be easy to copy-paste a command from Stack Overflow, when the use case that was asked about is totally different from your own. You’re used to these kinds of resources, and so am I.

But when it comes to writing lines of code that affect your entire project in a domain you don’t know much about, you need to reach out to someone with knowledge in the field.
