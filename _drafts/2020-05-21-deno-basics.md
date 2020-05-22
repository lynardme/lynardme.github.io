---
layout: "post"
title: "Deno Basics"
date: 2020-05-21
category: blog
tags: [deno, javascript]
---

Deno Features
* Use Typescript or Javascript
* Security by default
* De-centralized Packages
* Standard library
* Modern JS
* ES Modules
* Top Level/ First Class Await
* Built In Testing
* Browser Compatible API

#### Basic Server api call
``` javascript
import { Application, Router } from 'https://deno.land/x/oak/mod.ts'
const port = 5000
const app = new Application()
const router = new Router()
app.use(router.routes())
app.use(router.allowedMethods())
router.get('/api/v1/products', ({ response }: { response: any}) => {
    response.body = "Hello World"
})
console.log(`Server is running on port ${port}`)
await app.listen({ port })
```

