---
layout: "post"
title: "TMUX a terminal multiplexer"
date: 2020-05-03
category: dev
tags: [tmux, linux]
---

Yesterday, I wrote the blog [resizing tmux]({{ site.baseurl }}{% post_url 2020-05-02-resizing-tmux %}). Today, I will share more about TMUX and my experiences in this tool. 

TMUX in a nutshell is a terminal multiplexer that you can start a session and open multiple windows inside the session. It's really cool that you need to try it by yourself. 

Installing TMUX is as easy as 
```
sudo apt-get install tmux
```

##### Commands
```
tmux new -s session_name    -  create a new session   
tmux a                      -  attach the last session
tmux ls                     -  list
ctrl-b + d                  -  detach the session
```
