---
layout: post
title:      "React Project"
date:       2020-02-17 04:38:44 +0000
permalink:  react_project
---


Working through the react/redux final project truly felt like playing in a sandbox. It feels like a shiny new toy with endless exploration due to the constant work being done on it by Facebook and open source contributors. 

Here were some of the libraries/tools I played around with, and what they do:

<u>Redux Toolkit</u>

The name gives you a basic idea of what it does. It is a toolkit designed to reduce boilerplate code that plagues a lot of developers, while following conventions that the redux community has, such as the "Redux ducks" pattern. 

It uses a function called createSlice to, well, create a slice of redux state. It returns an object with a name property that all the reducer state will be nested under, the reducer itself, and an actions property that is mapped to an object of actions/action creators. These can then be exported to use in other files/components.

<u>React Hooks</u>

React hooks try to take away the complications that arise with class components, including lifecycle methods, compilation speed, and "wrapper hell." Hooks I decide to use were useState and useEffect from React; and useLocation, and useHistory from react-router.

I opted not to use redux hooks, as the benefits don't seem to be as apparent with them. For instance, you do not get the cacheing benefits that the connect wrapper provides, and their useSelector hook (which can be thought of as replacing mapStateToProps) feeds into the first problem by using different methods for comparing objects. The useDispatch hook also seemed a little extra when the connect wrapper binds your action creators to dispatch for you.

<u>Graphql</u>

One tool I really wanted to learn about with this project was graphql, a query language for api's that only returns exactly what you ask for. This prevents the classic over/under fetching problems that can occur with traditional api responses. 

I used yelp's graphql endpoint for this project, and it turned out to be a little tricky because they don't allow CORS requests...at all. Yelp's solution involved using apollo client, but even with that I would have had to make a Node.js or Rails backend. Since I was already using Rails, I just used that in combination with the graphql gem to have access the yelp's endpoint.

PHEW.

Here is an issue where a yelp dev also recommends a proxy api server: https://github.com/Yelp/yelp-fusion/issues/64.

<u>Conclusion</u>

All in all, this was a great project to learn some cool new concepts. In the future I need to add a user login feature to make my favorites feature work more fluidly. I would also like to play around with a data visualization library like D3.js.
