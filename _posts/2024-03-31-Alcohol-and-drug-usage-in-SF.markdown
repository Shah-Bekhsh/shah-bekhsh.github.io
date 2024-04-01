---
layout: post
title: "Alcohol and drug usage in San Francisco from 2003-2018"
date: 2024-03-31 12:30:14
subtitle: "How does substance abuse behave in San Francisco? A collection of insights and visualizations on the city's alcohol and drug usage. "
background: '/images/sf.jpg'

---

The dataset corresponding to San Francisco Police Reports includes incidents filed by police officers or citizens from 2003 to 2018. Containing data varying from geolocation of the crimes, date and time, to type of crime, this dataset carefully provides insights on how crime behaves in San Francisco for the given years, allowing us to deep dive in an interesting topic: alcohol and drug abuse in San Francisco.

We will try to understand how substance abuse has behaved in San Francisco, by showing different visualizations that one can easily identify patterns and insights from.


#### General overview

As a starter, we want to have a general overview on the ocurrence of alcohol and drugs related crimes reported in San Francisco from years 2003 to 2017.

![Calendar plot](/images/crimes_calendar.png){:style="max-width: 100%;"}

Analyzing the following calendar plot for the focused crimes per each day available in the dataset leads us to easily detect some interesting patterns.

- First, a peak in these crimes is easily observed during the years 2008 and 2009. This can be attributed to the financial crisis and recession that the United States was sustaining during these years, resulting in an increase of alcohol and drug usage. As mentioned in this article [^Crisis], financial crises are motivators that can lead to an increase in alcohol non-healthy consumption as a coping mechanism to psychological distress, which can be triggered specially by unemployment and income reductions.

- Highest rates are always during the first three months of the year, coincidentally, during winter. Winter conditions can have a huge impact on our psychology and behavior. Environmental factors, social isolation, holidays, and Seasonal Affective Disorder are some of the contributors to an increased substance usage, and could set a case for a deeper study on this topic [^Winter].

#### HeatMap (Pending)

The following heat map of the city over the years 2003 - 2017 demonstrates a few interesting trends over the years.

<iframe src="/time_heatmap.html" height="500" width="700" ></iframe>


#### Interaction
<iframe src="/Bokeh.html" height="500" width="700" style="border:none;"></iframe>

The interactive visualization presented above illustrates the incidence count of three distinct categories over time, with a specific emphasis on the yearly interval. The blue line, representing drug/narcotic incidents, exhibits a pronounced peak around 2008, followed by a gradual decline thereafter. The turquoise line, indicating drunkenness, alongside the green line, denoting driving under the influence, both maintain relatively stable but significantly lower incident counts over the same period.

Based on the strategic document of the United Nations Office on Drugs and Crime (UNODC) [^UNODC] for the 2008-2011 period, two key initiatives that might have contributed to the decline in drug-related crimes after 2008 are:
- Enhanced International Legal Frameworks: The strategy's emphasis on the universal ratification and implementation of international drug control conventions and improvement of national legislations could have significantly strengthened global efforts to combat drug-related crimes. The alignment of national laws with international standards likely resulted in more robust and effective legal actions against narcotics offenses.

- Intensified International Cooperation and Capacity Building: The UNODC's focus on increasing the capacity for international cooperation against organized crime, corruption, drug trafficking, and terrorism may have led to better coordinated and more comprehensive cross-border efforts to curb the illicit drug trade. The development of national criminal justice systems and the implementation of international legal instruments were vital in these cooperative efforts.

#### References

[^Crisis]: de Goeij, M. C. M., Suhrcke, M., Toffolutti, V., van de Mheen, D., Schoenmakers, T. M., & Kunst, A. E. (2015). How economic crises affect alcohol consumption and alcohol-related health problems: A realist systematic review. Social Science & Medicine, 131, 131-146. Retrieved from [https://doi.org/10.1016/j.socscimed.2015.02.025](https://doi.org/10.1016/j.socscimed.2015.02.025)
[^Winter]: "Why Do Drug Overdoses Increase in Winter?" _The Right Step Rehab Hill Country_. Retrieved from [https://www.rightsteprehabhillcountry.com/addiction-blog/why-do-drug-overdoses-increase-in-winter/](https://www.rightsteprehabhillcountry.com/addiction-blog/why-do-drug-overdoses-increase-in-winter/)

[^UNODC]: United Nations Office on Drugs and Crime. (2007). Strategy for the period 2008-2011 for the United Nations Office on Drugs and Crime. E/CN.7/2007/14–E/CN.15/2007/5. UNODC.