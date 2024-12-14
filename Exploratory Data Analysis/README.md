------------------------------------------------------------------------

# Exploratory data analysis of environmental conditions and marathon performance

### Background

This project is a collaboration with Dr. Brett Romano Ely and Dr. Matthew Ely from the Department of Health Sciences at Providence College. The report explores the relationship between environmental conditions and marathon performance. There's well documented sex difference between marathon performance and their response to environmental conditions. Age difference in marathon performance and their response to environmental conditions is also shown in previous studies. The data used in this analysis was collected from the 5 major marathons (Boston, Chicago, NYC, Twin Cities, and Grandma's).

### Methods

In this exploratory data analysis, the goal is to investigate (1) the effects of increasing age on marathon performance in men and women, (2) the impact of environmental conditions on marathon performance, and whether the impact differs across age and gender, and (3) which weather parameters (WBGT, Flag conditions, temperature, etc) that have the largest impact on marathon performance.

### Results

The analysis reveals the influence of environmental conditions, particularly black globe temperature, dry bulb temperature, wet bulb temperature, and dew point, on marathon performance. The relationship between WBGT and performance follows a U-shaped curve. Women experience a more accelerated decline in marathon performance as they age compared to men, especially in the 55-64 and 65+ age groups. The analysis also shows older age groups are more sensitive to heat and humidity, and therefore the impact of environmental conditions on marathon performance differs across age groups. Full report can be found [here](https://github.com/Miaoyanchen/PDA-Project-1/tree/main/Report%20files).

## Files

### Report files

-   `marathon_EDA_analysis.qmd` - R quarto file that contains the code for exploratory data analysis, such as summary tables and visualizations.
-   `marathon.bib` - Bibliography citation for references in the report
-   `marathon_EDA_analysis.pdf` - PDF version of the exploratory analysis report; code appendix is also available at the end of the report

## Dependencies

The following packages are required to run the code in the R quarto file:

-   `tidyverse` - data manipulation

-   `dplyr` - data manipulation

-   `ggplot2` - visualization

-   `kableExtra` - create nice table

-   `gtsummary` - create table summary and statistics

-   `lubridate` use to reformat dates
