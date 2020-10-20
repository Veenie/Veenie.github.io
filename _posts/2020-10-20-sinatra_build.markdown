---
layout: post
title:      "Sinatra Build"
date:       2020-10-20 22:08:52 +0000
permalink:  sinatra_build
---


Building out a wep app in Sinatra was a lot of fun! I built oan app the lets users sign up, sign in and sign out. Every user can create a collection of movies and assign them each a star rating using forms. They can create a new movie entry, look at it, edit it or choose to delete it. I also put protections in place so movie objects cannot be touched or seen by users who did not create them.

The gems involved were very handy, bcrypt made setting up passwords and encrypting them very easy (just gotta remember to call it password digest in my table!) Activereccord had many handy shortcuts as well, setting up my has_many and belongs_to set up many methods that were handy shortcuts, including verifying the presence of user inputs and validating that information entered is unique.

I think the helper methods set up in my application controller were the most handy thing of all, being able to use the logged_in? method and current_user methods really helped me secure the user's data. They can check that users are logged in and that the user session properly matches the data they want to access.

I'm really enjoying learning all these handy tricks, it is making my programming journey a lot easier and straight forward!
