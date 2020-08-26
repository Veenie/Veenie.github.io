---
layout: post
title:      "The CLI Project"
date:       2020-08-26 02:51:31 +0000
permalink:  the_cli_project
---


I am very excited to have completed my CLI project! I initially did an API based project but then I decided to try a scraper to challenge myself. There’s definitely a “Where’s Waldo” aspect to searching the website for code but I found it very informative. It taught me quite a bit on how websites are structured. I decided to build a CLI that would take episodes titles and descriptions from imdb.com to create a program that could function as an episode guide. A quick way to find an episode you have in mind but might not necessarily remember all the details of. I present the user with a numbered list of episodes and they can select the number to receive that episode’s description.

For this to work, I knew I would need to create episode objects in ruby that instantiated with the episode’s title and description which the scraped data could be plugged into. Once I had my episode class created and set to create objects, I created a class variable, @@all to store them in. Next, I gave my Episode class a class method .all that could not only show my class variable, it could tell ruby to scrape for my objects if the class variable was empty. Using a call to my scraping method in my Scraper class. The scraping method would in turn take the scraped data and iterate a loop that in turn plugged the data into new instance of an episode object.

Next came building my CLI. I wanted my commands to be simple so anyone could use it, even members of my family who are not computer literate. I kept the inputs limited to numbers and single lowercase letters. To start with, I had a call method in my CLI class that would be, well, called in my bin file. It in turn, calls on my methods to list my scraped episodes (using the aforementioned .all class method from my Episode class) and a method to take input from the user on the episode they want a description for. I made a method to display the description attribute from the chosen instance of the individual episode object. This also calls a method that allows the user to choose whether they want to see the list again or exit the program (this method is also called when the user puts in an invalid entry when choosing an episode.) I also made a method that does a validity check, the input must be greater than zero and a number that does not exceed the total number of objects.

I learned so much during this pod, just weeks ago I had never coded before. This accomplishment feels fantastic. I am really looking forward to my assessment as well, I look on refactoring my code as a great learning experience and working with a veteran will be very informative. I am happy to take on the challenge of changing what I already wrote and making it even better!

