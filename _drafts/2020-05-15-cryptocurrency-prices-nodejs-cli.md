---
layout: "post"
title: "Cryptocurrency Prices using NodeJS CLI"
date: 2020-05-15
category: dev
tags: [nodejs, cli, cryptocurrency]
---

I always fascinated about cryptocurrency even though I don't have any on my own but maybe someday I can try to buy this digital currency that is very trending now a days. 

This blog is all about how I tried to use an free API from nomics.com to get the cryptocurrency prices using nodejs in cli command like the one below. 
```
> coindex check price 
Coin: BTC (Bitcoin) | Price: $9,738.12 | Rank: 1
Coin: ETH (Ethereum) | Price: $202.29 | Rank: 2
Coin: XRP (Ripple) | Price: $0.20 | Rank: 3
```

Let's begin by getting the api from nomics.com

##### Get API key 
![](/assets/images/nomics-get-api-key.png){:class="img-fluid"} 
![](/assets/images/nomics-enter-email.png){:class="img-fluid"} 

##### To make the executable file a global command 

Put this line above in the file 
```
#!/usr/bin/env node
```
Next, we need to run `sudo npm link`. We want to make a symbolic link so that we can run anywhere the command. 

##### Install dependencies
