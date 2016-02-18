---
layout: post
title: "Accessing Plunker JavaScript variables in the console"
date: 2016-02-18
---

I really love <a href="http://plnkr.co" target="_blank">Plunker</a>. It's perfect for testing quick snippets of code. But it took me a while to figure 
out how to get access to my JavaScript inside of the console. Usually in the console, you can print out values in your 
JavaScript, but that doesn't work by default with Plunker. 

For example, below, I'm defining a variable, `myName` and then I'm trying to access it in my console, but it's 
`undefined`.

<img src="http://i.giphy.com/C7k4Gw0cF2kb6.gif" alt="GIF showing how Plunker JavaScript variables are inaccessible from the console" width="630px">

After playing around a little bit with the console, I figured out that you can easily fix this by just changing the 
the context from `<top frame>` to `plunkerPreviewTarget(run.plnkr.co/)`.

<img src="http://i.giphy.com/fSOGwRCPbZ06A.gif" alt="GIF showing how Plunker JavaScript variables are inaccessible from the console" width="630px">
