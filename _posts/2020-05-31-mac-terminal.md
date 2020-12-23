---
layout: "post"
title: "Mac terminal"
date: 2020-05-31
category: devtips
tags: [mac, terminal]
---

##### How to kill process locking port <number>

```
sudo lsof -i tcp:3000
kill -9 <PID>
```

##### Get ip address

> ipconfig getifaddr en0
