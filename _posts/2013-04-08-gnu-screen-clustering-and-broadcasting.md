---
layout: post
title: "gnu screen clustering and broadcasting"
description: ""
category: 
tags: []
---

This is about how you can send a command to multiple screen sessions.
This can work on byobu too since it is screen wrapped in rainbow.

to send the same command to all screen windows (per session)

enter command mode

C-a :

then execute

*at "#" stuff "command^M"*

where

at is a gnu screen command to label where to send inputs

means all windows

stuff = stuff the given string to selected windows

command is your given command

^M is to let screen know you are passing ENTER.

Examples:

This will send ls -l to all open screen windows in a session

at "#" stuff "ls -l^M"


