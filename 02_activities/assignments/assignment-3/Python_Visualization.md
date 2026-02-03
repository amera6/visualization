# Python / Jupyter Notebook Visualization (Line chart + Heatmap)

## 1) What software did you use to create your data visualization?
I created this visualization using Python in a Jupyter Notebook (edited in Visual Studio Code). I used the Python libraries `pandas` (data cleaning + grouping), `matplotlib` (line plot), and `seaborn` (heatmap styling and annotations).

## 2) Who is your intended audience?
My primary intended audience is public health and healthcare surveillance professionals, Toronto Public Health staff, and employees in hospitals, long-term care homes (LTCHs), and retirement homes. A secondary audience includes patients, residents, and family caregivers who want a clearer sense of *when* outbreaks are more common and *which settings* are most affected.

## 3) What information or message are you trying to convey with your visualization?
The main message is that outbreaks in Toronto healthcare institutions show seasonal variation across 2025, with higher counts during winter months and another rise around the beginning of the school year or early fall. The heatmap also highlights that long-term care homes (LTCHs) experience consistently higher outbreak counts than other settings, suggesting a setting-specific vulnerability and an opportunity for targeted prevention.

## 4) What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots?
I applied several design principles tied to aesthetics, perceptual clarity, and honest communication. First, I made sure to use the appropriate graph for my data and message. I used a line plot to communicate a time trend (monthly outbreak totals) because trends and seasonality are easier to perceive in lines than in bars. I used a heatmap to support comparison across two dimensions (month × outbreak setting), which helps the viewer quickly spot overburdened months and settings. In terms of perceptual effectiveness, the heatmap uses a perceptually-uniform sequential colour scale (I chose the reverse of rocket) to represent intensity, which matches the concept of “more = darker” and reduces ambiguity. I added cell annotations (numbers inside heatmap cells) so the exact counts are visible without forcing estimation from colour alone and avoids relying on colour only for conveying information. I rotated month labels and used month names (“January”, “February”, …) instead of “YYYY-MM” to reduce cognitive load and improve interpretability for non-technical audiences. I made sure titles were descriptive and include the place/time context (“Toronto healthcare institutions”, “2025”) so the plot can stand alone in a report. Both plots use the same month order and labels so the viewer can move between them smoothly: the line plot gives the big picture and the heatmap explains which settings contribute to peaks. In terms of substantive quality, I tried to honestly display the data by using counts (not proportions) and ensuring months are in chronological order. I avoided visual tricks like truncated axes for the line plot that could exaggerate differences.

## 5) How did you ensure that your data visualization is reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization?
I supported reproducibility by using a public dataset and documenting the data source: *Outbreaks in Toronto Healthcare Institutions* from the City of Toronto Open Data portal. Providing the full Python code used to import, clean, transform, and plot the data (including comments). I used deterministic transformations (e.g., `groupby`, `value_counts`, explicit month ordering) so that the notebook yields the same outputs when re-running it on the same dataset. Not maintaining reproducibility makes it harder to verify results, identify implicit assumptions, update visualizations when new data is released, or check errors from wrongful data cleaning.


## 6) How did you ensure that your data visualization is accessible?
I considered accessibility in several ways. First, I used text alternatives to convey information in the he heatmap (numeric annotations) which accomodates viewers who may have difficulty distinguishing colour intensity. I prioritizes Legible design choices like large figure dimensions, clear axis labels, and rotated month names for readability. I used a sequential colour map appropriate for low to high values. Finally, I kept the background clean (whitegrid setting) and did not overload the plots with extra decorative elements to minimize unnecessary clutter.

## 7) Who are the individuals and communities who might be impacted by your visualization?
This visualization may impact residents of long-term care homes and patients in hospitals who are often medically vulnerable (e.g., immunocompromised). It may also impact healthcare workers and support staff who face occupational exposure risks. Family caregivers and visitors are also impacted if they change visiting behavior during peak outbreak periods. Finally, public health decision-makers are impacted as they may use seasonal patterns to allocate staffing, PPE, and prevention efforts.

## 8) How did you choose which features of your chosen dataset to include or exclude from your visualization?

I included "Date Outbreak Began" which was converted into "Month" to examine seasonality. I used "Outbreak Setting" to compare patterns across hospitals, LTCHs, retirement homes, etc. Finally, "Counts of outbreaks", which was created by counting each row, was the quantitative value that directly answers the question of how many outbreaks occurred for each time period and setting. I excluded other fields such as institution names/addresses, specific causative agents, and outbreak end dates becuase they were either 1) not necessary for the seasonal message, or 2) would complicate the message and add another dimension beyond the main focus.


## 9) What “underwater labour” contributed to your final data visualization product?
Some of the hidden labour on my part that contributed to the visualization includes:
* cleaning and validating dates (`to_datetime`, removing invalid rows)
* creating and troubleshooting a reliable month extraction and ordering method (period month + month names) to avoid misordered categories
* iterating on readability like label rotation, figure sizing, switching from “YYYY-MM” to month names, and adding annotations to the heatmap
* checking for misleading defaults (e.g., ensuring months are chronological)
* writing code comments and documenting the dataset source so others can understand and reproduce the workflow

Some of the hidden labour from others include the healthcare institution staff who had to report outbreaks after identifying them, the surveillance workers at Toronto Public Health who recorded that information for surveillance purposes, and the data scientists who created and maintained the database of publicly available datasets.