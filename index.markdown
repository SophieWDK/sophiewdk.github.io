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

Our first visualization shows the total number of reported crimes per year from 2003 to 2025.

*(Insert time-series line chart or bar chart here)*

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/total_reported_crimes.png" style="width: 100%">
</div>

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/category_crimes_trend.png" style="width: 100%">
</div>

```python 
your_code = do_some_stuff
```



**Key Observations:**
- Crime peaked around **2006-2008**, coinciding with economic instability before the Great Recession.
- A sharp **decline occurs post-2014**, possibly due to increased policing strategies or changes in reporting.
- Certain crimes (like larceny theft) dominate, while violent crimes (like assault) remain relatively stable.

---

## **2. Mapping Crime Hotspots**  

Next, we map the density of crimes across San Francisco.  

*(Insert a heatmap or point-based map of crime locations)*  

**Key Findings:**  
- **Downtown (Tenderloin, Union Square, Market St.)** has the highest concentration of incidents.  
- **Residential neighborhoods (Sunset, Richmond)** see fewer reports.  
- Some clusters align with nightlife areas (Mission District) and transit hubs (Civic Center BART).  

---

## **3. Interactive Exploration: Crime by Category**  

Finally, let’s explore the distribution of different crime types interactively.  

*(Embed a Bokeh interactive plot—e.g., a bar chart or scatter plot where users can filter by crime category, year, or district)*  

**Try it yourself:**
- Filter by **"Larceny Theft"** to see its dominance.
- Compare **"Assault"** vs. **"Burglary"** trends over time.

---

## **Conclusion**

Crime in San Francisco has evolved over the years, with notable declines in certain categories post-2014. However, hotspots remain in high-traffic urban centers. Understanding these patterns helps policymakers and residents address safety concerns more effectively.

**Further Reading:**
- [SFPD Crime Data Dashboard](https://data.sfgov.org/Public-Safety)
- [San Francisco Chronicle: Crime Trends Analysis](https://www.sfchronicle.com)

*(Code and data available on [GitHub](your-repo-link))*