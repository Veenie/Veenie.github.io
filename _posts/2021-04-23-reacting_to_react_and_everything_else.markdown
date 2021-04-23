---
layout: post
title:      "Reacting to React (and everything else)"
date:       2021-04-23 11:47:57 -0400
permalink:  reacting_to_react_and_everything_else
---


It all built up to this, back when I began learning ruby I did not anticipate being able to do as much as I am now with React. It's great! I think the biggest takeaway I have from building my rails app is that one can do so much with a smaller amount of code. Yet at the same time it feels like the options for manipulating the functionality of my app. I've also had a lot of fun exploring how to style!

The way I structured things, I put the duty of passing the global state (via mapStatetoProps) on my container component. This allowed the child components, posts, to recieve the global sate for display. Container also handled my dispatch to fetch data to the backend. I think my post input component is what really demonstrates the flow of the app. Upon submission of a post, the data is sent to the action component. It's purpose is two fold: post to the backend via fetch and thanks to thunk we can chain a .then to dispatch the data as a payload in the action object sent to the reducer. Thus killng two birds with one stone.

When I look back at the bootcamp experience overall, I am very impressed with how far students can come in such a short time. I think my advice to future students would be to not stress if you don't understand things right away. I feel like it all comes together when you build your project. The lessons will handle teaching you all the pieces, but it's when you put them all together that you really understand how they flow together to make things work. Also, don't sleep on Ruby, the fundementals have come in handy countless times.

I think my favorite part of the program was the Rails section. It's when everything began feeling real and the things you are building feel very reminicent of the parts of the web we interact with everyday. I would encourage students to do their best to make it there, that's when things get really fun!
