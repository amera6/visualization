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

# January 27 - Session 4
## Lecture 7 Activities
### Slide 11 - Flatten the Curve Accessibility
The use of all capitals for the axes and graph titles can be hard to read for some individuals. Additionally, the use of red font to emphasize the start of early interventions may not be distinguishable for individuals who experience colour blindness. The lack of a subtitle/caption that explains the graph make it even more difficult for those who need additional contextual information or for those who use a screen reader.

### Slide 35 - Alt-Text Suggestion
A woman wearing a white lab coat and blue nitirle gloves (presumably a scientist) is speaking to a man in a blue, collared t-shirt. Both are standing beside a fume hood in a laboratory. The woman is standing on the left while the man is in the middle and the fume hood is on the right.

### Slide 39 - Four Types of Descriptive Content
Level 1 - This appears to be a stacked horizontal bar chart that acts as a timeline across the 24 hours in a day. The title says "The Daily Routines of Famous Creative People". The rows represent different famous people, while the columns represents an hour on the 12-hour clock (from 12am on the left to 12pm in the center and back to 12am on the far fight). Sections of the bar are coloured based on categories of different activities that can occur in the routine like sleep, food, exercise, etc.

Level 2 - The graph quantifies the relative proportion of each person's day that is made up of a specific activity. In terms of outliers, we can see that some people standout in terms of sleep (e.g., Mozart and Freud sleep the least while Flaubert and Styron go to bed the latest). Darwin exercises three times per day in short bursts while Dickens and Milton do one long workout. 

Level 3 - I don't notice any particularly trends aside from noticing that the people are arranged in order by the hour at which they wake up. I also notice that exercise was rarer among the creative people who lived in earlier time periods.

Level 4 - I don't have the particular domain insight for most of these creatives. I understand that they come from a variety of disciplines and time periods. The observation of exercise being rarer among earlier creatives makes me wonder if the concept of exercising voluntarily (for health or leisure reasons) is relatively new or limited to more priviledged groups.

## Lecture 8 (Slide 12) Activity
### How Rational, Moral, and Emotional Appeals are Used
Rational appeals are used by providing audiences facts about the dimensions of the cargo holds and the number of slaves on each tier. Both of which lead audiences to conclude that the ships were cramped and overcrowded beyond what is appropriate for its size and for human safety. 

Moral appeals are used by emphasizing key elements such as underlining the location of the slaves in the lower deck, likening the shelves to the galleries in churches, and juxtaposing the minimal space given to slaves against the large captain's cabin. The slaves are also drawn with details like clothes and faces to remind the audience that they are humans, rather than figures or bodies in a diagram.

An emotional appeal is made through the visualizations of the slaves, such as them crouching, crawling, and sitting slumped over to further solidify the lack of space that they have. They are also drawn laying down overlapping each other, as opposed to making them smaller to avoid overlap or showing them standing up in a top-down view. This further illustrates how crowded and innappropriate these conditions are for a population to live, sleep, and eat in. 


# January 29 - Session 5
## Lecture 9 Activities
### Slide 23 - Compare the two gender-related visualizations
The two visualizations communicate different types of evidence and support different kinds of interpretation. The mean-ratings chart (MacNell et al., 2015) compresses the data into a few summary statistics (group means with error bars) so it is designed to highlight a high-level comparison between actual and perceived instructor gender. In contrast, the gendered language visualization (Schmidt, 2015) is more exploratory. Instead of focusing on a single number, it shows patterns in word usage across groups and disciplines and encourages viewers to investigate how language differs. The advantage of the mean-ratings plot is that it is quick to read and supports a clear takeaway, but it can hide variation and context that may matter. The advantage of the language visualization is that it provides richer detail and can reveal nuance across categories, but it requires more effort to interpret and can be harder to summarize into a single message.

### Slide 32 - Types of changes in an interactive/dynamic visualization
Based on how the RateMyProfessor.com gendered-language visualization behaves in practice, the interaction produced by changing the search term is closer to an immediate change rather than purely identity-preserving or smoothly transitional. When the search term changes, the visualization doesn't just update points; it also reorders the y-axis categories (departments) and rescales the x-axis range substantially. Those are major spatial changes that make it harder to compare one query to the next. In contrast, several retinal encodings remain consistent across interactions, most importantly the colour mapping by gender group so the meaning of colour stays interpretable even as the spatial structure changes. If I were redesigning this visualization to improve comparability across searches, I would consider making the interaction more identity-preserving by keeping a fixed department order and providing a toggle between “fixed scale” and “auto scale”. That would make it easier to compare different search terms without the viewer having to mentally compensate for changing axes and reordered categories.