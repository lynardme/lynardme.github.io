---
layout: "post"
title: "TMUX hangs suddenly"
date: 2020-05-08
category: devtips
tags: [tmux, vim]
---

I have this weird behaviour while working in vim inside a tmux session. It's suddenly hangs and for no reason I couldn't enter any keys. The other window below is working which I run my program as output. Usually it hangs in the above window pane where VIM is running. 

It happened a few times and I didn't know what to do. I just close the tab of my terminal and open again all the application from my tmux window. Until I found a solution from this [stackoverflow](https://stackoverflow.com/questions/7408068/tmux-hangs-and-do-not-load-and-do-not-respond-to-any-option-command){:target="_blank"} 

The solution is very simple 

`ctrl-q`


