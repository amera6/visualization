# January 15 - Session 1 
## Lecture 2 (Slide 31) Activity
### Exploring Matplotlib
For this activity, I chose Graph #39 - Boxplot with Jitters. In terms of Aesthetics, I personally believe the graph is pleasing to look at but that is highly subjective and dependent on the colour palette used. The code from the gallery uses complementary colours of blue and orange which makes the jitters easier to view. 

Based on the description of the graph in the gallery, this graph appears to be substantive. It includes the basic boxplot which is useful for visualizing descriptive stats (like quartiles and outliers), but it also includes additional information about the underlying distribution for each boxplot and the number of observations (both of which are information that is lost in the basic boxplot). So, this visualization does accurately and honestly present the data. 

I think the one weakness of this visualization is its ability to convey its message to a lay audience. This perceptual gap comes from the fact that boxplots are already difficult to interpret unless you're well acquainted with statistical principles like distributions, skews, standard deviations, outliers, etc. Adding the dots on top could be informative to some viewers who desire a deeper understanding of the underlying distribution, but I believe that would be a smaller portion of the general audience who may misinterpret the jitters or find them to be overwhelming.


# January 20 - Session 2
## Lecture 4 (Slide 11) Activity
### Can Data Visualizations be Neutral?
In the first visualization ([US Gun Killings in 2018](https://guns.periscopic.com)) teaches us about the number of people in the US who died due to gun killings in 2018, but it also provides a lot of contextual information at the individual-level (the sex, race, age at death, predicted counterfactual age at death) and at the incident-level (gun type, number of victims, region, assailant type). The main narrative point of this visual is quantifying the number of potential life years lost for all victims. This makes the visualization non-neutral as it strongly emphasizes the harms caused by guns through a more emotional lens that centres individual victims who died. 

In contrast, the Washington Post Active Shooters graph only shows us an aggregated count of 'active shooter incidents' per year from 2000 to 2015. We get much less contextual information about each incident like the firearm type, region, number of victims, etc. We just get a sense of how many incidents occurred in the US across the years, and that these numbers fluctuated but ultimately display an upward trend. This image feels neutral in that there is minimal emotional charge behind the labels, such as labelling the gun carrier as an active shooter rather than an assaillant. 


# January 22 - Session 3
## Lecture 3 (Slide 21) Activity
### Comment Our Code
I went through the code and added comments that contextualize the purpose of each chunk (e.g., importing libraries, generating datasets, creating scatter plots, adding axes titles, customizing markers). I try to always have a main comment on the top of each cell in the jupyter notebook. I sometimes include more granular comments if there are code chunks within the same cell that each have different roles/purposes (e.g., setting graph theme, creating container and axes for figure, plotting variables, customizing graph elements). 

A good comment is one that helps walk a viewer through your decision-making process. This means adequately describing, and sometimes justifying, each additional element to the code that would make a meaningful difference towards the output. 


