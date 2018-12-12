---
layout: post
title: Breakpoint Failed to Bind - Visual Studio 2017
categories: [Blog]
tags: [Programming, VisualStudio, NoteToSelf]
---

Today I ran into an issue where I was trying to debug an application and I was getting a "Breakpoint failed to bind" error on Visual Studio 2017. I was trying to attach to the process when I got the error. I was already running in administrator mode, so it wasn't a permissions issue.

## Solution

Turns out I had the solution configuration set to "Release" right from the start. The solution then was to set the solution configuration 
to "Debug" and then rebuild the solution. After that, I was able to attach to the process with no errors whatsoever.
