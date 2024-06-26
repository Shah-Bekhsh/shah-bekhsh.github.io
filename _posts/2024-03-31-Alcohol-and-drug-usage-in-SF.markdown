---
layout: post
author: Shah, Daniel & Dan
title: "An Analysis of Substance Abuse in San Francisco from 2003-2018"
date: 2024-03-31 12:30:14
subtitle: "How does substance abuse manifest in San Francisco? A collection of analyzed patterns, visualizations and derived insights based on the city's alcohol and drug usage."
background: "/images/sf.jpg"
---

#### Introduction To The Dataset

San Francisco is the 13th largest city in the United States Of America. Its inhabitants include people from various cultural and ethnic backgrounds, including Asian, African American, Hispanic, and many more. With over 808,000 people living in the city since 2020, its no surprise that there is a lot of crime in San Francisco. In this article, we take a deep dive into a historical crime data published by the San Francisco Police Department (SFPD), from the years 2003 to 2018 ([DataSF](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry/about_data)), and statistically analyze the effects of substance abuse on the San Francisco community.

This dataset is a rich repository of information. It contains the information of each criminal incident that has been attended to by an officer of the SFPD, including the type of the crime, the time it was recorded, the geographical coordinates, and other such important details. Although, very useful, a lot of trends and insights remain hidden in this dataset. In this post, our goal is to analyze criminal incidents of substance abuse, including drugs/narcotics, liqour laws and other drunken behaviour, and try to identify whether there is a deeper connection with the underlying socio-economic factors.

#### Hotspots In San Francisco

Since the Great Depression, San Francisco has seen an almost impressive improvement in its economic situation. In 2023, the median income of a household in SF was roughly $153k. However, there is still a large income inequality between races, with almost 10.1% (mostly Black, Hispanic and Native Americans) of the inhabitants of the city living below poverty line. Unsurprisingly, this divide also shows in the regions of the city, occupied by low income inhabitants, where alcohol and drug related crimes are disproportionately high compared to the rest of the city. The Mission district in San Francisco is amongst the poorest districts in the city and its inhabitants are mainly Hispanic and Native Americans. Similarly, the Bayview district, which is a predominantly Black American neighborhood, also suffers from wealth inequality. And finally, we have the infamous region of Tenderloin, which we shall go into much deeper detail.

We map the drugs/narcotics and alcohol related incidents to the map of the city. This interactive map of the city shows the state of substance related crimes over the years (2003-2017). We can clearly see that areas with some of the lowest income are hotspots for crime. As described above, Mission district and Bayview district are the regions with high concentration of drug crimes.

<iframe src="/time_heatmap.html" height="500" width="100%"></iframe>

Let us now focus on Tenderloin, which is the worst affected region in SF due to drugs and the trend appears to be detriorating over the time. Throughout the years, the number of incidents have either remained constant or increased in this region. This can be attributed to an array of underlying social, economical and political circumstances. A survey [^survey] related to substance use, treatment and housing in Tenderloin reveals that this region has historically been a central location for many marginalized Americans (especially Black, Hispanic and Gay, Lesbian and Queer communities). Over the years, Tenderloin has become sort of a last resort for homeless and poverty ridden people of SF. Conversely, the areas around 19th Avenue, such as Sunset Dst, Forest Hill and Ocean View have some of the lowest incidents throughout the years. As seen in [this](https://sf.curbed.com/2016/12/9/13899936/income-inequality-map-san-francisco) blogpost, these are some of the highest income localities in the city of SF.

As such, a centralized drug market has been established in Tenderloin by the criminal element of SF, which preys on people with a history of substance abuse. The abundance of illicit drugs on the streets has ravaged Tenderloin the worst. The year 2023 (not shown in the heatmap), has been recorded as the deadliest year on record for drug overdose deaths in SF, with a state of emergency being declared in Tenderloin district.

#### Substance Abuse Incidents In San Francisco Over The Years

Let us take a step back and analyze the pattern over which the substance problem has evolved in SF. We use a calender plot to mark all the incidents that fall under the cateogories of "Liquor Laws", "Drugs/Narcotics", "Drunkenness" and "Driving Under Influence".

![Calendar plot](/images/crimes_calendar.png){:style="max-width: 100%;"}

This calendar plot immediately shows us some interesting patterns regarding the aforementioned categories of the crimes, which were not evident in the heatmap in the previous section.

- First, an increase in these crimes can be observed starting from 2006 until 2010, where it reached its peak of almost 12,000 incidents. Although it is very difficult to find the root cause to which this increase can be attributed, we believe that this issue was exacerbated by the housing market collapse of 2008 and the eventual global recession, which affected United States the worst. A lot of people across America lost their homes. The economic and social impact of this incident was extreme and devastated the psychological health of many residents of SF, causing an increase in the usage of drugs, alcohol and other illicit substances. This research article [^Crisis] reinforces our hypothesis, illustrating how financial crises can trigger severe psychological distress, potentially fostering unhealthy patterns of alcohol consumption and, in the most severe instances, drug addiction. Within communities experiencing financial upheaval, substances like alcohol and drugs often serve as affordable avenues for coping and seeking temporary relief.

- Highest rates are always during the first three months of the year and coincidentally, during winters. Winter conditions can have a strong impact on people's psychological health. Environmental factors, social isolation, holidays, and Seasonal Affective Disorder are also some contributors to an increase in substance usage during the winter season. We provide this article [^Winter] to support the correlation between winter season and substance abuse.

#### Facts & Figures

<iframe src="/Bokeh.html" height="500" width="700" style="border:none;"></iframe>

The interactive visualization presented above illustrates the incident count of 4 distinct crime categories over time, with a specific emphasis on the yearly interval. The blue line, representing drug/narcotic incidents, exhibits a pronounced peak around 2008, followed by a gradual decline thereafter. The turquoise line, indicating drunkenness, alongside the green line, denoting driving under the influence, both maintain relatively stable but significantly lower incident counts over the same period. Readers are encouraged to try changing the time interval drop down to observe the data in daily, weekly and monthly intervals.

Based on a document published by the United Nations Office on Drugs and Crime (UNODC) [^UNODC] for the 2008-2011 period, we can attribute this decline in drug-related crimes after 2008 to two key initiatives:

- Enhanced International Legal Frameworks: The strategy's emphasis on the universal ratification and implementation of international drug control conventions and improvement of national legislations could have significantly strengthened global efforts to combat drug-related crimes. The alignment of national laws with international standards likely resulted in more robust and effective legal actions against narcotics offenses.

- Intensified International Cooperation and Capacity Building: The UNODC's focus on increasing the capacity for international cooperation against organized crime, corruption, drug trafficking, and terrorism may have led to better coordinated and more comprehensive cross-border efforts to curb the illicit drug trade. The development of national criminal justice systems and the implementation of international legal instruments were vital in these cooperative efforts.

#### References

[^survey]: Chang, J. S. (2017). Health in the Tenderloin: A resident-guided study of substance use, treatment, and housing. Social Science & Medicine, 176, 166-174.
[^Crisis]: de Goeij, M. C. M., Suhrcke, M., Toffolutti, V., van de Mheen, D., Schoenmakers, T. M., & Kunst, A. E. (2015). How economic crises affect alcohol consumption and alcohol-related health problems: A realist systematic review. Social Science & Medicine, 131, 131-146. Retrieved from [https://doi.org/10.1016/j.socscimed.2015.02.025](https://doi.org/10.1016/j.socscimed.2015.02.025)
[^Winter]: "Why Do Drug Overdoses Increase in Winter?" _The Right Step Rehab Hill Country_. Retrieved from [https://www.rightsteprehabhillcountry.com/addiction-blog/why-do-drug-overdoses-increase-in-winter/](https://www.rightsteprehabhillcountry.com/addiction-blog/why-do-drug-overdoses-increase-in-winter/)
[^UNODC]: United Nations Office on Drugs and Crime. (2007). Strategy for the period 2008-2011 for the United Nations Office on Drugs and Crime. E/CN.7/2007/14–E/CN.15/2007/5. UNODC.
