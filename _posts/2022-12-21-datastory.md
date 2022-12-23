---
layout: post
title:  "A story of women's representation in the movie industry"
date:   2022-12-21 17:56:05 +0100
background: '/img/Actress_pic.jpg'
---
The last decade has been marked by emancipating and feminist movements. While many inequalities subsist to this day, women’s rights have progressed, along with mentalities[1][2].
As a result, the lack of women’s representation in far too many domains was put in the spotlight and could no longer be ignored. In this context, we consider that the film industry could be viewed as a reflection of society across time and space. Indeed, the cinema industry is a product of spectators’ expectations and social norms. However, it also impacts the viewer and can participate in popularizing new scenarios and characters, which can have a significant social impact in the long term. 


In this context, we propose to study movies dating from 1940 to 2009 from the CMU corpus and attempt to derive trends and specificities of female characters to understand the evolution of women’s representation. This analysis might help us determine whether the recent movements were preceded by an underlying improvement of women’s condition as reflected in the film industry, or whether these movements marked a societal gap. 
We will study women’s representation in the whole movie industry throughout the last century and further assess how much our observations are conserved according to two of the most important characteristics for each movie: its genre and the country in which it has been produced. 

 

##### Global representation of women in the movie industry

The evolution of women’s representation can be observed under three different scopes: their relative presence in the movie industry, the character’s traits such as age, and finally, the role given to female characters and their involvement in the plot.

To set the stage, let’s look at the proportion of roles played by women in the whole set of movies.  

![general_pie](https://pauldfepfl.github.io/DatastoryNonNansLand/img/general_pie.svg)

Obviously, something is wrong, maybe this ratio has evolved through time, and recent ratios are closer to equity! So let’s look at it to settle the situation:



![cnt_prop_gen](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Count_proportion_general.svg) 

Even if we might observe an increasing trend, statistically, there is no significant difference in proportions of female characters between decades. We are far from reaching 50% of female characters on average. Additionally, women’s representation can be studied from different scopes, for example, the main attribute of actresses, one of them being age distribution. Our first intuition would be that female actresses tend to be younger than male actors, but numbers are better than words: 


{% include_relative age_distribution.html %}
Once again a clear tendency appears, and confirms our intuition. Looking at different decades (using the interactive plot), we observe that throughout the last century, women’s age distribution has always been shifted towards a younger age compared to men. It tends to get better, but overall, actresses are younger on average than their male colleagues even though they have the same range of age represented. This highlights quite a significant attribute that sticks to female characters, they are younger and this gives already a hierarchical ascendancy to their masculine fellows. This also might be a symptom of the well-known female hypersexualization in visual content [3]. Then, to get better insights on their importance in the movie, we can analyze what the movies’ summaries say about their role and their ability to make the plot go. To do so, we chose 3 metrics: the agent and patient verbs and the attributes associated with a character. 


Respective examples could be:
To explain those three 3 metrics, in the following sentences *kill* can take different values: 
- Mary has *killed* Dr. Jones (agent verb)
- Mary was *killed* by Dr. Jones (patient verb)
- Mary is a *killer* (attribute)


{% include_relative word_proportion_general.html %}

This graph shows the average percentage of allocation of words to women per movie, i.e., at 50%, each woman has as many words allocated to her as each man, independently of the number of female or male characters. We can observe that overall, each female character is almost as much described as each male character, with an allocation varying between 40 and 50%. That’s good news! Even though women are less present, when they are, they seem to be well-mentioned in the plot. 
We have now determined that female characters are depicted with a similar amount of words to male characters. However, we have no clue how those words are used. From what we know, there could just be a high amount of words used to undermine women’s representation or their relevance in the plot. Therefore, let’s have a qualitative view of the words used to characterize women over time. These word clouds are generated on the entire dataset for the 1940’s and 2000’s movies.


![wc3](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudAV.png)

We start by observing the agent verbs, as they can be more informative about the character’s importance. We notice that on the surface, those graphs are very similar overall, with the same top words. Looking in details, we notice that between the 1940’s and 2000’s, new words were introduced to describe women which used to be only attributed to men, such as ‘confront, ‘manage’, and ‘shoot’, while others, such as ‘marry’ disappeared, highlighting a slight but noticeable shift of female importance towards more active words over time.



![wc2](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudPV.png)

Then, secondary characters could gather a high amount of words, which would be passive as the character would not make the plot go forward. Here, in opposition to agent verbs, we notice a difference in quantity between male and female characters. Indeed, we can see in the 1940s that female characters are extensively described with more diverse patient verbs, but the top words are the same for both genders. Whereas, terms like ‘love’, ‘marry’, and ‘jealous’ are more attributed to female characters, while ‘shoot’ and ‘capture’ are missing, this configuration inverses in the recent decades. 
Even though it is subtle, we notice an evolution in words used to describe women towards words that are less passive and that were typically used for men. 



##### Analysis by genre

As the movie industry is very diverse, women’s representation might be very different from one movie to another. Try to think, which female character first comes to your mind when you visualize an action movie, and how does it compare to a typical romantic female character? In this context, we propose to study if our previous observations on the whole cinema industry are conserved across the different movie genres. As many movies belong to several genres at a time, we chose to analyze three movie genres that are as independent from each other as possible, i.e., Action, Horror, and Romance. First, let’s look at the different female characters proportions in each genre:

![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Genres.png)

Although not all genres display the same proportions of female characters, women are once again strongly under-represented, especially in action movies. Then, we can have a look at the other aspects of women’s representation to see if they also differ according to the genre, starting by the age distributions of the female and male actors.

![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/age_genre.svg)

Women are invariably younger than their colleagues. However, the situation is not the same among genres, with romance being the only genre with a real improvement, trying to bridge this gap in the past hundred years.
Finally, it is interesting to watch how women’s description varies across genres.


{% include_relative word_proportion_genres.html %}

Once again, separating by genres shows that looking at the general data can be deceiving. Looking at the word distribution by character, we can see that the women in action movies receive significantly fewer words than male characters. There is an increase in women’s importance in the plots, nonetheless it stays relatively small compared to romantic movies, in which it seems intuitive to give similar relative importance to women and men.
Knowing that the number of words evolve in different manners according to the movie genre, we can once again assess the words associated with women:



![wc](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudRA.png)

Interesting, isn’t it? As expected, the lexical fields differ from one movie genre to another. Here, we can see an overall similarity across time, but also between female and male characters. Even if female characters are under-represented as shown above, we can see that, in the 2000s, action movies seem to be depicting similarly female and male characters. We notice larger words such as ‘kill’ and ‘tell’, as well as the apparition of words such as ‘leave’, ‘take’, ‘save’, ‘help’ and ‘meet’ compared to the 1970’s movies. 

On the other hand, we can see that words in romance movies vary less through time and are consistent between genders. It is in line with our previous findings that romance movies show the most equal results. Indeed, we do not see the appearance of top words to the extent of action movies. Instead, some words such as ‘find’, ‘make’, ‘decide’, already present in the 1940s for both genders, became more important.



##### Geographical analysis

Until now, our analysis depicts a rather sad picture concerning the representation of women in the movie industry. Our intuition is that not every country presents the same gender inequalities. Therefore, we looked at movies produced by the two biggest movie industries worldwide: Hollywood and Bollywood, to see if women representation is homogeneous all around the world.  
First, we can quantitatively assess the relative women’s representation. To do so, let’s look at the overall count of female characters in Indian movies by decade, compared to movies produced in the US. As one can see, there are more female characters in the US due to the fact that our dataset contained more movies produced there. The proportions of women however have only slightly changed, with a small increase trend for the last decades. 



![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/Count_proportion_geographical.svg)

We now know that the proportion of women is similar in both countries, around 35%. Age distribution of female actresses in both countries remains to be seen. Note that since we are comparing countries that might have very different demographics, we also included the life expectancy throughout the last century per country to allow a proper comparison of the average actresses' age.

![a](https://pauldfepfl.github.io/DatastoryNonNansLand/img/age_geograph.svg)

The average male and female actors' ages do not change significantly throughout the last century in the US, where the life expectancy is always above 60 years old. On the other hand, the average Indian actors' and actresses’ age increases over decades, following the rapidly rising life expectancy from 1920 to 1960. As soon as the life expectancy reaches 50 years old in the 1970s (reached in the 1920s for the US) the average age of actors and actresses reaches a plateau. Even though the population is aging, the film industry seems consistently attached to having relatively young persons on the screen, and even younger females. It is worth mentioning that the difference in average age in the US (although clearly visible) is still smaller than in Indian movies.  
  

Knowing that the relative presence of female and male actors might not be representative of their respective characters’ importance, we performed a last language analysis. As one can see, the percentage of words allocated to female characters in American movies slightly varies over the decades. There are no significant changes over the whole century, female characters being described with only around 40% of the total descriptive words. However, there is a significant diminution of the percentages of words used to describe women in Indian movies, going against the trend of increasing female characters’ presence.


{% include_relative word_proportion_geograph.html %}

We have seen that women’s representation follows different trends according to genres. The preceding analysis shows that the origin of the movie also has an impact on the type of word used compared to the overall analysis. Once more, due to the major part of the movies in the dataset originating from the US, general results could have hidden underlying effects. Let’s have a look!


![wc](https://pauldfepfl.github.io/DatastoryNonNansLand/img/wordcloudIA.png) 

It is hard to miss the words ‘daughter’ and ‘marry’ which were central in the Indian 1960s, reflecting a patronizing environment. In turn, the US resembles, as expected, the overall analysis. Indian female characters’ evolution is the most striking we’ve seen so far amongst all word clouds.
Indeed, the words ‘daughter’ and ‘marry’ are significantly reduced to leave room for independence-related words such as ‘decide’, ‘begin’, ‘ask’ and ‘think’.  We can see that the Indian word clouds greatly shifted towards words used to depict male characters in general. Finally, we also notice, to a lesser extent, an evolution in American movies, with more active words such as ‘decide’, ‘discover’ and ‘explain’. We can see that the Indian film industry has made undeniable progress and got closer to the Hollywood’s standards of considering women. Nevertheless, women are not yet considered equally to men in the plots.


##### Conclusion

To answer our initial question: How has the representation of female characters evolved in the film industry over time? We examined the dataset through different scopes and further separated movies by their characteristics, such as the movie genre and country of origin. Women are increasingly being better represented in the scenery, with more leading roles and more nuanced and realistic characterization. This is important for promoting gender equality and challenging harmful stereotypes. However, this is not a general statement. Indeed, this trend did not follow a straight path, and varied from the nature of the movie to the place it was produced. This relative evolution is still not enough to attest equality in the film industry, even for the latest movies. Recent movements for gender equality may help to accelerate progress in the future. It is crucial for the film industry to continue to strive for more diverse and accurate representation of women to better reflect reality and promote gender equality.


 

[1] https://www.womengoingbeyond.org/post/milestones-for-feminism-from-the-last-decade
[2] https://www.forbes.com/sites/lizelting/2019/12/20/the-2010s-the-decade-women-fought-back/?sh=68c5546421ad
[3] LUOYING YANG
