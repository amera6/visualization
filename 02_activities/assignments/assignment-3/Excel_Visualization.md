# Excel Visualization (Stacked Bar Chart)

## 1) What software did you use to create your data visualization?
I created this visualization using Microsoft Excel in an Excel Worksheet. I used Excel’s built-in chart tools and a PivotTable to aggregate the dataset into counts by outbreak setting and outbreak type, then visualized those counts as a stacked bar chart.

## 2) Who is your intended audience?
The intended audience is primarily infection prevention and control (IPAC) staff, outbreak surveillance personnel, and healthcare administrators who need a quick snapshot of outbreak burden by setting. A secondary audience includes patients, residents, and family caregivers who may benefit from a high-level understanding of which settings experience the most outbreaks.

## 3) What information or message are you trying to convey with your visualization?
This visualization is meant to communicate differences in outbreak burden across healthcare settings in 2025, and to show how that burden breaks down by outbreak type (respiratory vs enteric). The stacked design makes it easy to see which settings have the highest total outbreaks overall, and whether those outbreaks are dominated by respiratory or enteric causes. This can support prioritized resource allocation (e.g., settings with consistently high totals may need additional vigilance, staffing, PPE).

## 4) What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots?
Key design choices were made to maximize quick comparison and reduce misinterpretation. The stacked bar chart was chosen to the answer the question because it effectively compares totals and compositions at the same time (total outbreaks by and setting  respiratory vs enteric share). 

I ensured perceptual clarity by using high-contrast colours plus patterns for the two outbreak types. The patterns help distinguish categories even when printed in grayscale or viewed by people with colour-vision differences. The y-axis starts at zero which supports honest comparison of magnitudes. 

I added large data labels so viewers don’t have to estimate values from the axis. The title states the what/where/when clearly (“Ontario,” “2025,” “by setting and type”). Both of these elements reduce cognitive load on the viewer.

## 5) How did you ensure that your data visualization is reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization?
Excel is less reproducible than a scripted workflow because some steps can be done manually and may not be recorded (filtering, cleaning, reformatting), and different users can accidentally alter cells.

To improve reproducibility, I used a PivotTable (instead of editing raw data directly), which preserves the original rows and makes aggregation logic visible (fields, filters, rows/columns). I included a source citation directly on the figure which points to the dataset location.

Due to this limited reproducibility, if someone recreates the chart without the exact same pivot configuration (or if the dataset updates), their totals may differ. Also, since manual steps are harder to audit than code, transparency is reduced and results become harder to validate.


## 6) How did you ensure that your data visualization is accessible?
I supported accessibility by using patterns and colour (not colour alone) to distinguish outbreak types, adding data labels so exact values are visible without relying on colour perception, keeping text sizes large and legible, and ensuring the layout remains interpretable even if printed in grayscale.

## 7) Who are the individuals and communities who might be impacted by your visualization?
This chart may influence how different groups understand outbreak risk and preparedness needs. Residents and patients in long-term care and retirement homes may be more vigilant of any respiratory or gastro symptoms. Family caregivers may use this visual to decide when/how to visit/ Healthcare workers and support staff at higher-risk sites may employ more strict infection prevention and control (IPAC) protocols. Finally, outbreak management teams and decision-makers may choose how to allocate prevention resources based on this visual.

Because the chart could affect perceptions of specific settings, it’s important to communicate that these are reported outbreaks and that reporting practices and population differences (size, vulnerability, institutional structure) may also shape the counts.

## 8) How did you choose which features of your chosen dataset to include or exclude from your visualization?
I included "Outbreak Setting" to compare burden across healthcare environments, "Type of Outbreak" (respiratory vs enteric) to show the composition of total outbreaks within each setting, and I calculated the count of outbreaks from the rows to use as the main metric (simple and interpretable).

I excluded specific institution names and addresses because they're not needed for the high-level comparison and could create stigma against certain settings. I also didn't include organism/causative agent because it would add complexity and distract from the main message of setting burden. Finally, time trends (month-by-month) were excluded because this chart is meant as a cross-setting summary rather than a seasonality analysis.

## 9) What “underwater labour” contributed to your final data visualization product?
Some of the hidden labour on my part that contributed to the visualization includes:
* converting the CSV dataset into an Excel worksheet and verifying that key fields (e.g., Outbreak Setting and Type of Outbreak) were consistent enough to summarize
* deciding on an aggregation approach (counting outbreaks by setting and type) and building a PivotTable
* validating the PivotTable output (spot-checking totals and categories) to ensure the chart reflected the underlying data accurately
* iterating on readability and accessibility choices such as chart title wording, axis labels, legend placement, font sizing, and adding data labels
* selecting high-contrast colours and patterns to distinguish respiratory vs enteric outbreaks 

Some of the hidden labour from others include the healthcare institution staff who monitored for outbreaks and reported them, the surveillance staff (e.g., at public health units) who received and recorded those reports, and the people responsible for cleaning, maintaining, and publishing the dataset through the open data portal.