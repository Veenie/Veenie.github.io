---
layout: post
title:      "Console logging away!"
date:       2021-02-23 20:27:14 +0000
permalink:  console_logging_away
---


For my single page application, I choose to make an app that allows users to fill out a form so they can leave quick impressions or "hot takes" on a movie. I am utilizing a Movie class and Review class, with movie functioning in an orginzational way: the review is assigned or "belongs to" that film. The review is what the user can construct and manipulate.

Besides a form to construct reviews, the page does a get fetch to the rails api to display existing reviews created in the database. Upon filling out the form and submitting it, a post fetch is run to take the entered data and add it to the database on the backend. It is also run through a constructor, using OOJS, to make a js object version of the review so it can be immeadiatley rendered to the DOM without having to do a page reload or another fetch. I also included the ability to call a deletion endpoint so reviews can be removed from that database, as well as removing it from the DOM by using remove() on the parent element in js.

Using the browser console was very invaluable during the process. Finding and manipulating the correct elements was very crucial and I appreciated that there is a lot of flexibility in js, you can find many possible solutions to what is in front of you. Rails is very standardized, which is a very good thing, wherhas js does allow for flexibility and creativity.
