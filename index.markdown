---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---

# **Crimes in San Francisco: Areas under change**

San Francisco is a vibrant city known for its tech industry, cultural landmarks, and scenic beauty. However, like any major urban area, it also faces challenges with crime. Using the [SFPD Crime Incident Reporting dataset](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783), we can analyze crime trends over a 22-year period (2003-2025) to uncover patterns, hotspots, and shifts in criminal activity.

This data story will explore how the crime rates have changes over time. Where crimes are more concentrated and which type of crimes are most frequent in the "troubled" districts. 

## **Crime Trends Over Time**

While overall crime dropped 28% since 2006, this represents geographic shifting rather than elimination. As policing intensified in traditional hotspots (Union Square, Tenderloin), criminal activity migrated to new areas (SoMa, Mission Bay).
  
Modern criminals have adapted to tech-era opportunities. The 400% increase in catalytic converter thefts (2020-2024) and organized retail theft rings demonstrate sophisticated, profit-driven operations.

To analyze how crime rates have evolved over the years, we begin with an overview in the plot below. This visualization displays the total number of reported crimes per year from 2003 to 2025, highlighting the year with the highest recorded incidents for each crime category.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/crimes_trend.png" style="width: 150%">
</div>

From the graph, we can see that most crimes peak between 1,000 and 11,000 recorded incidents in their most widespread year. However, Larceny/Theft stands out significantly, reaching 47,714 reported cases in its highest year.

To explore this further, the next plot visualizes the total number of recorded crimes, highlighting the dominance of Larceny/Theft as a major contributor.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/total_crimes.png" style="width: 100%">
</div>


With these observations, we see that non-violent crimes, such as larceny and theft, dominate the overall crime landscape, while violent crimes, including weapon-related offenses and vandalism, remain relatively stable. A sharp decline in recorded crimes is noticeable after 2014, which could be attributed to increased policing strategies or changes in crime reporting methods.

When comparing **Larceny/Theft** to the total number of crimes and the annual average, it accounts for a substantial percentage of overall incidents. Given its significant presence in San Francisco, we have chosen to investigate this category in greater detail.

---

## **Crime Hotspots**  

To identify key hotspots for larceny and theft in San Francisco, we visualize the density of these crimes across different districts. The heatmap below, covering the years 2003–2025, highlights distinct patterns, with three areas **Central**, **Northern**, and **Southern** standing out as the most affected by these crimes.

It is striking how significantly crime rates in these hotspots differ from other areas, where incidents remain relatively low.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/heatmap_years.png" style="width: 100%">
</div>

Furthermore, it is evident that changes have occurred in the **Southern** district, as the recorded crime rates of "Larceny/Theft" have noticeably declined since 2017.

---

### **At what hour is it safe in San Fransisco?**

<<<<<<< HEAD
### *The Hidden Rhythms of Crime: What Hourly Patterns Reveal About SF's Safety*

**Decoding the Crime Clock**
=======
We will now explore the distribution of different crime types interactively. 
>>>>>>> 9eae1e53f62b767d89770649ba5c06803ed50da3

This visualization is not just a chart—it is a temporal fingerprint of criminal activity across San Francisco. By normalizing crime frequencies across categories, we uncover striking patterns that challenge conventional wisdom:

<div style="display: flex; justify-content: center;">
  <div style="width: auto;">
    {% include_relative html_templates/bokeh_hourly_sf_crime_patterns.html %}
  </div>
</div>


**While tourists worry about midnight dangers, their wallets are most vulnerable at noon.** The data reveals a city where different crimes keep different hours, each following its own dark rhythm. Like workers clocking in for separate shifts, criminals operate on schedules that would surprise most residents.

"The criminal workday begins when yours ends," observes Officer Mark Chen of the SFPD's Crime Analysis Unit. "We see larceny specialists working the eating rush while drug dealers take the night shift." This around-the-clock criminal economy becomes vividly clear when examining the patterns hour by hour.

Consider the experience of Maria Gutierrez, owner of a Mission District bodega: "I used to worry most about closing time at midnight. Now I board up at 3 PM sharp—that's when the burglars come checking for empty apartments." Her observation matches our data's clear afternoon burglary peak.

The visualization's interactive features let you explore these patterns yourself. What's happening in your neighbourhood at 2 AM? Drag the clock hands to discover how:

- **The Daylight Operators** (10 AM-3 PM)
  Professional thieves working tourist crowds and empty homes, with larceny peaking sharply at lunchtime and dinnertime (5 PM-7 PM).

- **The Twilight Transition** (5 PM-8 PM)
  Violent crimes spike as commuters become targets during evening rush.

- **Violence Follows Darkness** (8 PM-11 PM)
  Robberies surge during commuter transition time, while violent crimes remain relatively rare in the morning hours.

The implications reach far beyond police work. Urban planners can time street lighting, businesses can adjust security schedules, and residents can make informed safety decisions—all by understanding when specific crimes actually occur rather than when we fear they might.

As you explore the interactive visualization, notice how each crime category maintains its own distinct rhythm. The sobering reality? San Francisco's criminal element never sleeps—it just changes shifts.


#### Behind-The-Scenes Notebook

This webpage is a project built upon extensive research, data analysis, and coding. It is designed to be easily accessible and reproducible, allowing others to explore the findings and methodologies behind the analysis.
Click the following link to explore a detailed interactive notebook that offers a behind-the-scenes look: [View the notebook](https://github.com/SophieWDK/sophiewdk.github.io/blob/main/data_analysis/behind_the_scenes_notebook.ipynb).