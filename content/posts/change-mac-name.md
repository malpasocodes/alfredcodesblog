+++ 

date = 2023-11-25
title = "Change Macintosh Computer Name"
description = ""
slug = ""
tags = ["MacOS"]
series = ["MacOS"]

+++

As a developer, you are constantly working in the terminal environment. If you use a Macintosh, Apple annoyingly sets the computer name to something like "Mycroft's Blah Blah". If you hunt around in "System Settings", you will sooner later come across "General", then "About". There you can change the name of the computer to something you want. You think you are home free, but that doesn't change the name that appears on the command line in terminal. There are also other places where the name change doesn't propagate. 

Here's the way to change the hostname of your computer across the board:

{{< highlight python >}}
sudo scutil --set ComputerName "newname"
sudo scutil --set LocalHostName "newname"
sudo scutil --set HostName "newname"

{{</highlight >}}

For good measure, you should restart your computer after applying the changes. 
