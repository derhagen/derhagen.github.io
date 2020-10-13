---
layout: post
title: Video Conferencing is broken for many physical scenarios
---

Most video conferencing systems generally assume the same physical usage scenario: We have n users who sit or lie around in distinct physical locations, each of them having a client device to participate in an n:n video call, i.e. everyone can talk to everyone. Even though some platforms came up with a designated presenter or breakout rooms, I haven't seen the assumptions of the physical separation challenged yet. Thereby, we have been struggling with different physical scenarios for a while. People who have a conference room at their workplace, that is just too large for a conference phone, know the terrible "catch box", a soft wireless microphone cube that is thrown from speaker to speaker, but is also magically attracted by half-empty coffee cups.

## 1. The classroom

A very similar setup comes up, now that university classes start again, with some students attending in-class and some online: If questions come up from the students in class, either the lecturer repeats them out loud, or we start passing microphones around for discussions. One of my fellow students came up with the idea to just follow the class both online and in-class. When we want so speak, we can unmute our laptop/phones, so the online participants can hear it. Unfortunately, in order to avoid feedback loops, the lecturer has to mute the room speakers, that we need to hear them. A lively discussion involving both groups of students is not really possible, this way.

## 2. The study group

There are more scenarios where a similar problem comes up: Students meet up physically in small, decentralized study groups to participate in an online lecture together. This is not a problem, as long as only one laptop is used, but this becomes difficult if you have to maintain a distance to each other. So each of us watches the lecture on their own laptop, with all but one having their speakers muted -- or using headphones. Again, if one of us is asking a question, we have to mute the speaker/headphones in order to avoid feedback loops or to not hear the speaker in the room twice: Once in reality, a second later in the stream.

## A solution proposal

Overcoming the first problem would be as easy as introducing a "microphone-only"-mode to video conferencing systems in the following way: Online participants join the conference in the usual way, whereas students sitting in the classroom or lecture hall join in the "microphone-only" mode that simply provides a basic push-to-talk functionality, nothing else. Assuming that the conference host is the one that controls the room speakers, the conferencing system could play the audio stream from students in class only to those participants that are not the host -- and not "microphone-only", of course. That's basically a selective BYOD room-wide microphone array for each classroom that does not require any installation. Who needs expensive conference room installations any more, when a beamer, a speaker and n laptops or phones are all we need?

To solve the second problem, we can generalize this approach, but this requires our system to have a more detailed awareness of the physical context, i.e. which participants are in the same room with each other. While it would certainly be possible to figure this out automatically, as long as one device per room has their speakers enabled to send an identifying audio signal to the others, it would be sufficient to manually group clients if they are in the same room, so none of them hears the audio from the others -- at least not through the video call. In the same way we don't want to hear our own voice in the call, which we probably take for granted, but which means that some kind of client-specific selection of the audio streams already happens, anyway. This functionality would just have to be generalized to the set of other clients in the physical room.
