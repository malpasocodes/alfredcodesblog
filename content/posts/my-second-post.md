+++ 

date = 2023-11-28T10:00:37-05:00
title = "My second post"
description = ""
slug = ""
authors = []
tags = []
categories = []
externalLink = ""
series = []
+++
This is my second post. Let's see if we can add Python code.


{{< highlight python >}}

class hello_sayer:
    def __init__(self, greeting = "Hello"):
        self.greeting = greeting
    def say_hello(self, name):
        print(f"{self.greeting}, {name}!")

if __name__ == "__main__":
    h = hello_sayer("Good morning")
    h.say_hello("Jeff")

{{</highlight >}}



