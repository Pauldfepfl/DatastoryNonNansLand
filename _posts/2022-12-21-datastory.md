---
layout: post
title:  "A story of women's representation in the movie industry"
date:   2022-12-21 17:56:05 +0100
background: '/img/Actress_pic.jpg'
---
The last decade has been marked by emancipating and feminist movements. While many inequalities subsist to this day, women’s rights have progressed, along with mentalities[SOURCE ?].
As a result, the lack of women’s representation in far too many domains was put in the spotlight and can no longer be ignored. In this context, we consider that the film industry could be viewed as a reflection of society across time and space. Indeed, the cinema industry is a product of spectators’ expectations and social norms. However, it also impacts the viewer and can participate in popularizing new scenarios and characters, which can have a significant social impact in the long term. 

In this context, we propose to study movies dating from 1940 to 2009 from the CMU corpus and attempt to derive trends and specificities of female characters to understand the evolution of women’s representation. This analysis might help us determine whether the recent movements were preceded by an underlying improvement of women’s condition as reflected in the film industry or whether these movements marked a societal gap. 
The evolution of women’s representation can be observed under three different scopes: the character’s traits such as age, their presence in the movie industry related to the number of female characters, and finally, the role given to female characters and their involvement in the plot.
 

##### Global representation of women in the movie industry

To set the stage, let’s look at the proportion of roles played by women in the whole set of movies.  

![general_pie](https://pauldfepfl.github.io/DatastoryNonNansLand/img/general_pie.svg)

Obviously, something is wrong, this ratio must have evolved between decades, and recent ratios should tend to equity! So let’s look at it to settle the situation:


![cnt_prop_gen](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Count_proportion_general.svg) 

Even if we might observe an increasing trend, statistically, there is no significant difference in proportions of female characters between decades. We are far from reaching 50% of female characters on average. However, women’s representation can be studied from different scopes, one of them being age distribution. Our first intuition would be that female actresses tend to be younger than male actors, but numbers are better than words: 

{% include_relative age_distribution.html %}
Once again a clear tendency appears, and confirms our intuition. We can also look at the age distribution per decade (using the interactive plot). Throughout the last century, women’s age distribution has been shifted towards a younger age compared to men. It tends to get better, but overall, actresses are younger on average than their male colleagues even though they have the same range of age represented. This highlights quite a significant attribute that sticks to female characters, they are younger and this gives already a hierarchical ascendancy to their masculine fellows. This also might be a symptom of the well-known female hypersexualization in visual content  [LUOYING YANG]. Then, to get better insights on their importance in the movie, we can analyze what the movies’ summaries say about their role and their ability to make the plot go. To do so, we chose 3 metrics: the agent and patient verbs and the attributes associated with a character. 

Respective examples could be:
To explain those three 3 metrics, in the following sentences *kill* can take different values: 
- Mary has *killed* Dr. Jones ![JONES](/img/LES_JONES)(agent verb)
- Mary was *killed* by Dr. Jones (patient verb)
- Mary is a *killer* (attribute)


{% include_relative word_proportion_general.html %}

This graph shows the average percentage of allocation of words to women per movie, i.e., at 50%, each woman has as many words allocated to her as each man, independently of the number of female or male characters. We can observe that overall, each female character is almost as much described as each male character, with an allocation varying between 40 and 50%. That’s good news! Even though women are less present, when they are present, they are well-mentioned in the plot. 

We have now determined that female characters are depicted with a similar amount of words to male characters. However, we have no clue how those words are used. From what we know, there could just be a high amount of words used to undermine women’s representation or their relevance in the plot. Therefore, let’s have a qualitative view of the words used to characterize women over time. These word clouds are generated on the entire dataset for the 1940’s and 2000’s movies.

![wc3](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudAV.png)

We start by observing the agent verbs, as they can be more revealing of the character’s importance. We notice that on the surface, those graphs are very similar overall, with the same top words. Looking in detail, we notice that between the 1940’s and 2000’s, new words were introduced to describe women which used to be only attributed to men, such as ‘confront, ‘manage’, and ‘shoot’, while others, such as ‘marry’ disappeared, highlighting a slight but noticeable shift of female importance towards more active words over time.


![wc2](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudPV.png)

Then, characters can also be depicted as secondary and could gather a high amount of words, which would be passive as the character would not make the plot go forward. Here, in opposition to agent verbs, we notice a difference in quantity between male and female characters. Indeed, we can see in 1940’s that female characters are extensively described with more diverse patient verbs, but the top words are the same. Whereas, terms like ‘love’, ‘marry’, and ‘jealous’ are more attributed to female characters, while ‘’shoot’ and ‘capture’ are missing, this trend inverses in the recent decades. 
Even though it is subtle, we notice an evolution in words used to describe women towards words that are less passive and that were typically used for men. 

The diversity of the dataset could have covered these subtle differences. Indeed, Movie genre and movie origin, which are more extensive in the dataset, potentially hid some more specific results by smoothening the analysis.


##### Analysis by genre


{% include_relative word_proportion_geograph2.html %}
{% include_relative word_proportion_genres1.html %}


{% include_relative Count_proportion_general.html %}
![wc3](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloud3.jpg) 
![wc2](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloud2.jpg) 
![wc](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloud.jpg) 

![b](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Count_proportion_genres.jpeg)
![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Count_proportion_geographical.jpeg)
![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Genres.png)
![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/US_India_pie.png)

![wc3](/img/wordcloudRA.png) 
 
 
![wc](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudIA.png) 
![wc](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudRA.png) 
