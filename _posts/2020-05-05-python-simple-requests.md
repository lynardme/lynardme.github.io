---
layout: "post"
title: "Python Requests Module"
date: 2020-05-05
category: dev
tags: [python, requests]
---

Requests is a module that you can use to send all kinds of HTTP requests

###### Basic request
```python
import requests
r = requests.get("https://api.github.com/repos/psf/requests")
print(r.json()["description"])
```
###### Auth request
```python
import requests
r = requests.get('https://api.github.com/user', auth=('username', 'password'))
print(r.status_code)
print(r.headers['content-type'])
print(r.encoding)
print(r.text)
print(r.json())
```
