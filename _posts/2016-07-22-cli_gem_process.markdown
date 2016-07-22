---
layout: post
title:  "CLI Gem Process"
date:   2016-07-22 02:17:34 +0000
---


Where to begin! So this process was interesting. I was blazing through the lesson plans with no issue for the most part. However once you step out of the lessons and start actually stubbing out some full fledged code, things can trip you up. 

My thought process on creating a gem was to make something I thought could be beneficial even if it was simple. After getting some inspiration from the Learn slack channel, I decided on creating a gem that scrapped hospitals in the area. Since I live in DC, scrapping the hospitals here wouldn't be that difficult. I also wouldn't have had to think through an iteration method for the purposes of scrapping too many hospitals contact data!

I first decided to get the gem package so that I could have a lot of the depencies and file structure ready to go. That took a lot of the heavy lifting out so that I could focus on actually creating the interface for the command line. My focus was to build the relative file structures out as it related to feeding the bin (executable) file. Building out the library was a great process in allowing myself to visualize the logical flow of the gem.

First I started to build out the lib file that housed most of logical path of the gem. Creating an overarching method that showcased the logical flow of the other methods was a great start. I then worked through building out the file that housed a lot of the nokogiri code (after I added the depency of course). It was here that I needed to come up with the process of scraping the data I found from a DC Hospital listing website. The trouble I encoutered here was how to do so when the values I wanted were presented in a table (tr) form. I kept pulling in empty strings and I couldn't figure out why. 

It was only after playing around with it for so long that I was able to figure out that I needed to incorporate indexing in order to retrieve the correct values. Once I was able to get that going I then looked to utilize instance variables so that I could incorporate that and instantiate the values retrieved into a message to shoot back to the user.

Once I started to work on the goodbye message, I reflected on the project from the beginning. Like anything in life, starting from the beginning is tough. I definitely had a hard time trying to think of ideas for the project as well as what I wanted the user to see. However once I got past that initial hurdle, I started to appreciate the "try it, break it" approach. It became surprisingly fun to see what worked and what didn't work logic wise. Doing so allowed me to arrive at a working application (my first!), and I'm exciting to apply this to the future projects I work on here at Learn and beyond. 
