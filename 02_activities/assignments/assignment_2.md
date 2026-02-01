# Data Visualization

## Assignment 2: Good and Bad Data Visualization

### Requirements:

- Data visualizations are important tools for communication and convincing; we need to be able to evaluate the ways that data are presented in visual form to be critical consumers of information 
- To test your evaluation skills, locate two public data visualizations online, one good and one bad  
    - You can find data visualizations at https://public.tableau.com/app/discover or https://datavizproject.com/, or anywhere else you like! 
- For each visualization (good and bad):  
    - Explain (with reference to material covered up to date, along with readings and other scholarly sources, as needed) why you classified that visualization the way you did.
      ```
      A visualization that I believe to be very good is one by Alberto Lucas Lopez, a former journalist and Senior Artist at National Geographic. His visualization on [Past Pandemics](https://www.lucasinfografia.com/Past-Pandemics) does a great job conveying lots of information in an easy-to-navigate infographic. Each pandemic or epidemic is visualized by a triangle. He uses the x-axis to represent time in multiple ways. First, the width of each triangle is scaled to indicate the duration of the outbreak. Second, he orders the triangles from left to right to indicate their temporality, with the left-most outbreak starting the earliest. He measures the y-axis in terms of estimated deaths (in millions), so the height of each triangle represents the severity of the outbreaks. Other elements such as the colours (for scales of outbreak) and symbols (for animal source and pathogen name) add more information without cluttering the space. Finally, he includes little blurbs for each outbreak to add more context and he connects these blurbs to the triangles using a dotted line. The strategic use of size, the incorporation of context clues via symbols, and the intentional placement of text are all practices encouraged by Tableau for effective visualizations ([source](https://www.tableau.com/visualization/data-visualization-best-practices)). Additionally, the prioritized use of length (vertical and horizontal) and relative position for conveying most of the information aligns with John Hopkin's Sheridan Libraries' guide on precise quantitative information ([source](https://guides.library.jhu.edu/datavisualization/design)). I also believe this visualization succeeds in all aspects of visualization quality (aesthetics, substantive, perceptual). The graph is pleasnt to look at with a good amount of negative space, a limited colour pallet, and an easy to read legent. The graph honestly represents the data in terms of the duration, severity, and primary source of the outbreaks. Finally, the visualization uses plain language and simple elements to show the scale of past pandemics/epidemics and seems easy to understand for a general audience.
      
      One visualization from the same artist that I believe is bad is [this one](https://www.lucasinfografia.com/Mortality-causes) showing the top 10 causes of mortality across the richest and poorest countries in the world. The top graph shows a circle composed of multiple wedges, each representing a country, with the wedges on the left showing the 20 poorest countries in the world, and the right showing the 20 richest. The wedges have 10 segments that are each labelled with a cause of death (ex., Ischemic Heart Disease). At the center of the circle, there is a list of the most common causes of mortality among the poorest and richest countries, separately. Below this graph, there are a few secondary graphs that demonstrate patterns in mortality across countries for a given cause. Finally, they show the top 10 causes of mortality for different regions of the world, as well as globally. While this visualization shows important information, I think it utilizes visual elements in a way that's unintuitive. For example, the top visualization indicates that the ordering of mortality causes starts on the inner-most segment of the wedge and continues outwards. Intuitively, I would associate the largest segment of the wedge, which is the outer-most, as corresponding to the top/largest value of the variable (cause of death). Additionally, the circle layout of the main visualization leads to an awkward reading experience as one has to turn their head and read side-ways for most of the countries, while also dealing with a switch in orientation of the labels at the 3-o'clock and 9-o'clock positions of the circle. This can be jarring as the viewer would need to immediately turn their head all the way over to the other side to read the subsequent wedges. This greatly reduces the readability of the visualization for viewers with limited neck mobility. The graph uses too many variables, colours, and graph labels which can become overwhelming and confusing to the viewer at first glace, as demonstrated by this [Statistics Canada guide for data visualzation](https://www150.statcan.gc.ca/n1/pub/89-26-0005/892600052022001-eng.htm). The graph utilizes more imprecise ways of visualizing quantitative information, such as width ([Sheridan Libraries](https://guides.library.jhu.edu/datavisualization/design)). I believe the data visualization is not very aesthetically pleasing due to how overwhelming it is. I also believe it doesn't convey the key message to viewers in the most efficient way due to the circular orientation of the graph and the unintuitive use of sizing. I don't know enough of the background information to comment on its substantive quality, but the grouping of countries based on wealth is a little misleading when realizing that wealth is based on GDP rather than GDP per capita (based on the sources at the bottom). Many of the countries listed as being "the poorest" are very small island nations in Oceania and the Caribbeans. I think there are better measures of economic wealth that could've been used when comparing countries of vastly different population sizes.
      ```
    - How could this data visualization have been improved?  
      ```
      First, I think the information could be presented just as effectively as a stacked bar chart rather than a circle. The y-axis could measure the proportion of all mortalities attributed to a single source, such that the stacks for each bar sums up to 100% (one stack would need to be a catch-all for non-major causes of deaths). I think each group of 20 countries could have its own graph. I also think the definition of economic wealth should be made explicit through a note on the graph. I think the secondary visualization could remain as is, although a map of the regions that have a given cause of mortality in its "top ten" would be more informative of global trends. 
      
      ```
- Word count should not exceed (as a maximum) 500 words for each visualization (i.e. 
300 words for your good example and 500 for your bad example)

### Why am I doing this assignment?:

- This assignment ensures active participation in the course, and assesses the learning outcomes
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story

### Rubric:

| Component               | Scoring   | Requirement                                                 |
|-------------------------|-----------|-------------------------------------------------------------|
| Data viz classification and justification | Complete/Incomplete | - Data viz are clearly classified as good or bad<br />- At least three reasons for each classification are provided<br />- Reasoning is supported by course content or scholarly sources |
| Suggested improvements  | Complete/Incomplete | - At least two suggestions for improvement<br />- Suggestions are supported by course content or scholarly sources |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 01/26/2026`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (assignment_2.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-2`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
