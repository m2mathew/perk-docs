---
title: howhap-middleware requires an express session.
description: howhap-middleware requires an express session.
date: 2016-02-20
layout: topic.html
order: 100
---

[howhap-middleware](https://github.com/alarner/howhap-middleware) is a library that makes it easier to display errors from the server to the client. This library assumes that there is an express session available on your request objects. The above error commonly occurs if your session configuration is incorrect or your redis server is not running.

### To fix

Try running `redis-cli` on on the command line. If you get an error that looks something like:

```
Could not connect to Redis at 127.0.0.1:6379: Connection refused
```

then you need to start your redis server.