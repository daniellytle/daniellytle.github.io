---
layout: post
title: Exploring how brands have existed in hip-hop
date: 2019-08-04 12:02 -0600
categories: writing data-science
---

I found a [MetroLyrics dataset](https://www.kaggle.com/gyani95/380000-lyrics-from-metrolyrics) on Kaggle and was curious about specific mentions of brands in different genres. I was especially curious about Hip-hop and wanted to find a quantifiable example of trend changes over time. Specifically when, did Cristal gain popularity? Is Hennessey still mentioned in modern music? Let's look at the lyrics written by Easy E, 50 Cent, and Tupac to track the mentions of these brands through their rise and eventual fall.

### The Dataset

Only analyzing songs tagged as "Hip-Hop" gives us 266,556 songs spread out across 25 years (1991 - 2015). The distribution of data is not uniform across the years so I normalized results by dividing the number of songs with mentions of a certain word by the number of songs in our data from that specific year.

![](/assets/img/data.png)

## Analysis

The main investigation was to take a category that's often referenced in Hip-Hop songs and track the popularity of specific brand values in that category. I picked the categories of drinks, drugs, and guns to investigate. Within these categories, I looked for values I knew from modern music as well as older terms I expected to occur in earlier songs.

### Drinks

In this category I looked at four terms: Diddy's Ciroc, the famed Cristal, Hennessey, and Patron. The resulting graph looked to confirm my suspicions. Cristal and Hennessey are the only brands to be mentioned before the mid 2000s, most likely because they were around before the others, people have been drinking Hennessey and Cristal for centuries, Patron debuted in 1989, and finally Ciroc arrived in 2003.

![](/assets/img/drinks.png)

It's around the mid-to-late 2000s that we see the newcomers Ciroc and Patron start to take some attention from the old favorites. Ciroc and Patron peak around the 2010 mark then join the other brands in a steady decline towards modern day. It's an interesting change which might be explained by our next investigation, as rap stars put down the bottle for something a little stronger.

### Party Drugs

When we do the same analysis with common drug terms we see a massive rise in popularity after 2010. Referencing party drugs in songs has recently become much more mainstream. I looked for usage of the terms: "Xan" (Xanax, an anxiety medication), "Purp" (a term for purple drink or codeine), "Percocete" (painkiller), "Codeine" (cough syrup), and "Molly" (a term for MDMA).

![](/assets/img/drugs.png)

Artists like Lil Xan and Yung Lean, are recording millions of plays on Spotify. Even popular Hip-Hop artists like Drake and Travis Scott include drug references in their hit "Sicko Mode", which spent 30 weeks in the Billboard Top 10 Chart.

### Guns

Another aspect of Hip-Hop culture the aggressive rivalries that clash outside of the studio. Artists often speak to this lifestyle in their music. I was curious if artists had a particular brand of choice when it came to weapons. For analysis I picked the terms: Uzi, Glock, Ruger, and AK.

![](/assets/img/guns.png)

The results showed and early preference for the Uzi and the AK, while Glock jumped up with high popularity starting in the early 90s, peaking in 2000, and remaining relevant today. It's interesting to note that in the year 2000, "Glock" appeared in our data in over 10% of songs. This may be attributed to a rhyme-able brand name but nonetheless, the small handgun is by far the most popular gun in Hip-Hop.

### Limitations

- We assumed our data to be a random sample of Hip-Hop songs throughout the past 20 years in order to identify overall trends. We would be able to claim to see trends with more confidence if we had data on all Top 40 songs of the last 20 years.
