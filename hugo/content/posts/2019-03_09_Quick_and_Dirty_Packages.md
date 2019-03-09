+++
date = "2019-03-09"
draft = false
title = """Quick and Dirty Packages"""
slug = "quick-and-dirty-packages"
description = "Introduction to modular thinking in python"
keywords = "programming,python,packages,modularity"
tags = ['Programming', 'Python']
+++

{{% toc %}} 

Imagine a smartphone app that is used like a type of glue to assist in accomplishing difficult or mundane tasks in other, possibly larger, applications. Now imagine multiples of these micro-applications all the tips of your fingers. Each of these micro-applications can do one thing exactly the same way every single time.

Welcome to programming in [python](http://bit.ly/2SSKKEL), and more precisely, welcome to a quick and dirty introductory blurb on [modularity](http://bit.ly/2EWIwAc) in python using [PyPI](http://bit.ly/2EOaoVZ) and [pip](http://bit.ly/2SSuYJO), the dynamic-duo for finding and downloading python [packages](http://bit.ly/2NSzI1h).

The main purpose of a package in python is to modularly separate out logic, allowing one to leverage pre-existing code (that you or another person wrote and maintain) to complete routine tasks in your application or script. This can range from displaying characters [upsidedown](http://bit.ly/2EYlxVC) on the command line or in your flagship application being seen by billions of visitors every day, to more useful functions such as calculating the tragectory of your favorite pitchers curve ball in near real time using [MDAnalysis](http://bit.ly/2tZ4tsh) simulations.

Using pip to install the packages provided on PyPI alone will not get you the results you are looking for -- that will require some [general programming logic](http://bit.ly/2J2ikZg) to stitch it all together.

To truly understand the power of modularity and packages, and why you may want to use them, start by looking at problems with a problem-solvers perspective:

1. Identify what you have -- You have information (data). This could be anything and from any source. For example: user input, a form, a database, published data scraped from a competitors website, etc.
2. Identify what you want to do with the data -- extract just the useful information, encrypt the file, backup to another disk, send the information to another application (json/xml payload), store the data in a database, etc.
3. Find a tool that already does part or all of what you want to accomplish -- Is there already a tool to help you achieve the results that you are looking for? This can be broken down many times. In fact it very much is. We often need to combine features from multiple packages to perform a larger operation on a [data set](http://bit.ly/2tYUYt4) for a specific outcome.

This article focuses on step #3, discoverying tools which have already been built for you to complete the task at hand. I gave 2 examples above for transforming arbitrary text and applying calculus. With this simple thought experiment, and python of course, a person with no programming experience can pick up a rather abstract problem, break it down into it's simplest form, and have a working solution within a few minutes to a couple of hours. I'd suggest setting your sights relatively low, and work up your general programming skills as you develop more useful and interesting projects, leveraging what has already been built for you. We are focusing on speed to solution here in step 3, perfection does not exist, and we don't care about [optimization]. Remember that you are building a tool to solve your particular problem, much like a blacksmith or metalworker would craft a pickaxe for the sole purpose of mining.

Like every other problem that exists (in programming and not), input must be provided. In the examples above, our input is text and the result is the text being displaying upside down, and there could be several inputs for the curveball trajectory simulation -- one could imagine such an [algorithm](http://bit.ly/2J04aI8) (read "step-by-step process") taking into account parameters such as the weather, elevation, throwing motion and fatigue, the force of gravity, jersey number and so on.

Think liberally for a few seconds about any problem and you'll quickly realize that it is created by a single or multiple contributing factor(s), and there's an outcome to everything (though you may not appreciate the outcome). This is a programming truth as well. Some packages you find in PyPI will not support the number of required input parameters for the problem you are trying to solve, for example. In such a case, there may be another package available that supports a more robust use case. You will want to review the [standard library](http://bit.ly/2TCzDUz) of packages that come [builtin](http://bit.ly/2J2fNON) to python.

Generally, you may find multiple options of packages that you can leverage to solve your problem. If you don't find exaclty what you're looking for then you have a few options:

1. Pick the package that most closely fits your use case and re-write it to support the functionality that you desire. -- This is often more trouble than it's worth. I mention it first to illustrate that we can use brute force but there are often times a more ellegant approach. If you do go through with this and get it working, try making a [pull request](http://bit.ly/2EYPB3k) against the maintainer's version of the code (usually in [github](http://bit.ly/2u0H4q8)).
2. Invent the wheel. -- I humbly write that it's doubtful your use case is so unique that a package doesn't already exist to help you solve it, especially if you're reading this to learn about PyPI and pip, so this path should not be chosen unless you really want to recreate a package for learning sake. In that case, more power to you!
3. Rethink your problem. -- PyPI hosts 171,334 packages at the time of me writing this. Are you sure your problem isn't solved already? Try expanding your search, and even try [googling](http://bit.ly/2HmlwfO) to see the solutions other people have tried. You can always find a package and then circle back to see if the package exists on PyPI and can be installed on your machine using pip.
4. Don't use pip. -- Piggybacking off of #3, it's possible that your problem is solved on github or another corner of the web, and the maintainer just didn't add it to PyPI. If you end up going this route, try contacting the maintainer of the snippet your using, and see about getting the project on PyPI to help others. Chances are, if the code is publicly available on the internet already, they're interested in helping others and will oblige.

If you choose option 2, consider publishing your package on PyPI to help others. If it's [proprietary code](http://bit.ly/2SUWhmF), seek approval for an [open source license](http://bit.ly/2SQo7Ax) through your company, suggest one that best fits the philosophy of your company.

Please be generous to folks writing packages and posting them on the internet, many of them are just trying to help and are doing it free of charge. If something isn't working the way you expect it to be working, take a few moments and seriously contemplate the issue you're seeing. When you understand what isn't working, try to fix it. Google the error you're seeing in the output of your program. Developers time is important so consider how you're using the package and the error(s) or unexpected results you receive [before reaching out to them](http://bit.ly/2SSRtP1). The python community is full of people willing to help. [Stackoverflow](http://bit.ly/2Tp3oZQ), [Quora](http://bit.ly/2SSRtP1), or even a friendly [Facebook python group](http://bit.ly/2SOM5MN). If all else fails ping me.

A client of mine recently asked, how quickly can you teach me to do what you do? This article is not intended to be a copypasta to teach people pip, [virtual envs](http://bit.ly/2UtjKgB), [imports](http://bit.ly/2STINrA) in python, nor [programming fundamentals](http://bit.ly/2Jfrq55) and [data structures](http://bit.ly/2TGe7yn). The internet is full of resources from  articles, tutorials, videos, free courses and pdfs, which I pointed my friend to as well. This is a beginners introduction into the [mindset](https://amzn.to/2SVkEkm) of why you may want to use external python packages (or understand the power of a modular approach to problem solving) and how you will inevitably benefit from using PyPI and pip as a [developer](http://bit.ly/2tWoH5R), [tinkerer](https://aol.it/2CaqFnO), or otherwise [curious](http://bit.ly/2EZMWqi) person. If you've never used python before, I strongly encourage you to check out [python.org](bit.ly/2SSKKEL), [talkpython.fm](http://bit.ly/2NTop91), and search [youtube](http://bit.ly/2CeiGpA) for python related videos (youtube was originally written in python, though idk to what extent python is currently being used there).

Finally, I leave you with this [happy little ai-ccident](https://youtu.be/5DaVnriHhPc).

Until next time.
