---
layout: post
title:      "Using Axios to fetch"
date:       2020-02-25 04:33:45 +0000
permalink:  using_axios_to_fetch
---


Javascript's native fetch is good and all, but some bits of it can be cumbersome. Take for instance this basic fetch code: 

```
const getDataWithFetch = async (url) => {
  const resp = await fetch(url);
	const data = await resp.json();
	return json;
}
```

The previous code takes a url, makes a request, then turns the response to json. However small, boilerplate like this can add up in programs. Now let's look at axios performing the same action:

```
import axios from 'axios';
const getDataWithAxios = async (url) => {
  const data = await axios.get(url);
	return data;
}
```

Wow, we skipped a whole step! Not only that, but the axios "get" function makes our code more readable. Normally in fetch requests, you would have to sift through the configuration of the fetch request to discern what it was doing. Not anymore. Axios has other useful aliases, as well, such as axios.post.

What about fetch calls that take basically the same configuration? Axios allows us to make an instance of it with cusomized configuration, like headers. You can then import this instance into any file in your program where you need it. Handy!

Error handling, canceling requests, and interceptors are other features to play around with. I recommend everyone try it. 
