---
layout: post
title:      "A speed date with Graphql"
date:       2020-02-26 01:00:14 +0000
permalink:  a_speed_date_with_graphql
---


A curious thing has been popping up lately as I go to use api's for my projects: a lot of companies are beginning to play around with graphql endpoints for their api.

Graphql is a query language that lets you fetch the exact data you need -- no more, no less. This prevents the classic over/underfetch problems of the past, which makes requests easier to parse and harder to flood your program with. 

For example, if you wanted to fetch a particular user so you could view their name, then fetch their posts with metadata, and finally fetch the posts' likes, it might look like this:

```
const user = fetch('/users/<id>');
const posts = fetch('/users/<id>/posts');
const postLikes = posts.map((post) => fetch('/posts/<postId>/likes'));
```

That's a lot of fetches for just one page, and doesn't even include us having to parse it for the information we want. Let's look at this with graphql:

```
{ query {
  user(id: <id>) {
	  name
	  posts {
		  datePublished
			views
		  likes {
			  author
			}
		}
	}
}
```

All the same data with one request and more readable/succinct code.

However, there can be downsides to graphql. LogRockets mentions the following: 
1. REST can do much of what GraphQL does
2. GraphQL will make some tasks more complex
3. It’s easier to use a web cache with REST than with GraphQL
4. You could have performance issues with GraphQL queries
5. The way GraphQL schemas work could be a problem

## Conclusion

Graphql is a great tool, but it is just that -- another tool. Take care to use graphql to solve the right problems, without introducing worse ones. With many companies, like yelp and github, moving to graphql endpoints, it is definitely worth learning the basics of this technology.

