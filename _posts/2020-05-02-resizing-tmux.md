---
layout: "post"
title: "Resizing Tmux"
date: 2020-05-02
category: blog
tags: [tmux,tags]
---
Previously when I wrote Java programs I use eclipse as my IDE. There is a separation of files explorer, the editor and the terminal output at the bottom. It's make your life as a programmer easier. I was happy at that time contended as a Java programmer. But things changed since last 6 years ago. I used different programming language like python, javascript, etc. I'm also comfortable using linux commands and editor called VIM. 

Since then, I love using VIM as my editor but once in a while I use a graphical editor like sublime. 

So, I'm wondering if I can able to copy the setup from my eclipse before and use only linux terminal, of course VIM as the editor but with the terminal running at the bottom. 

I have found out that TMUX could allow you have multiple terminal sessions running simultaneously in a single window. After couple of research in the internet I found the right command to split the window and resize. 

```
ctrl-b + "      -- to split horizontal
ctrl-b + :      -- waiting for command to execute
:resize-pane -D 10
```
![](/assets/images/resize-tmux.png){:class="img-fluid"} 

#### Switch panes
Below command able you to switch focus
```
ctrl-b + o      -- transfer focus to the next window
```

But, suddenly I accidentaly switch the panes of top and bottom. 

![](/assets/images/switch-panes-tmux.png){:class="img-fluid"} 

#### Disaster, haha.

To switch the panes or rather the command that I accidentaly press is 
```
ctrl-b + alt-o
```

That's all folks, if you have similar experience and want to share with me I'm happy to talk about it. Follow me at [@lynarddotme](https://twitter.com/lynarddotme){:target="_blank"}. Thanks!

See references:
- [https://tmuxcheatsheet.com/](https://tmuxcheatsheet.com/){:target="_blank"} 
- [https://gist.github.com/henrik/1967800](https://gist.github.com/henrik/1967800){:target="_blank"}

