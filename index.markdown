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

## **Interactive Exploration: Crime by Category**  

We will now explore the distribution of different crime types interactively.  

<script>
fetch('/html_templates/bokeh_hourly_sf_crime_patterns.html')
    .then(function(response) { return response.json() })
    .then(function(item) { return Bokeh.embed.embed_item(item) })
</script>

*(Embed a Bokeh interactive plot—e.g., a bar chart or scatter plot where users can filter by crime category, year, or district)*  


### *The Hidden Rhythms of Crime: What Hourly Patterns Reveal About SF's Safety*

**Decoding the Crime Clock**

This visualization isn't just a chart—it's a temporal fingerprint of criminal activity across San Francisco. By normalizing crime frequencies across categories, we uncover striking patterns that challenge conventional wisdom:

**Key Revelations from the Clock**

1. *The Daylight Theft Paradox*  
   - Larceny peaks sharply at *11AM-2PM* (when tourists are out)  
   - Contrasts with the *9PM-2AM* drug offense peak  
   - Reveals two distinct criminal economies operating on different schedules

2. *Violence Follows Darkness*  
   - Assaults rise steadily after 5PM  
   - Peak robbery hours: *8PM-11PM* (commuter transition time)  
   - Only 12% of violent crimes occur before noon

3. *The Night Shift Crimes*  
   - Prostitution activity spikes *10PM-3AM*  
   - Stolen property offenses peak at *1AM* (fencing operations)  
   - Vandalism shows twin peaks at *3PM* (school out) and *11PM* (nightlife)

---

### *Three Business Models of Crime*

**1. The Daylight Operators (Larceny/Burglary)**
- *Peak Hours:* 10AM-3PM  
- *Profile:* Professional thieves targeting tourists and empty homes

**2. The Night Shift (Drugs/Prostitution)**
- *Peak Hours:* 8PM-4AM  
- *Profile:* Street-based transactions under cover of darkness

**3. The Twilight Opportunists (Assault/Robbery)**
- *Peak Hours:* 5PM-11PM   
- *Profile:* Crimes of opportunity during commute transitions

---

From here on I'd delete everything and we can build up on that maybe?

### *Policy Implications*

1. *Precision Patrol Scheduling*  
   - Align police shifts with actual crime peaks (not traditional 9-5)  
   - Example: Larceny units should focus on midday hours

2. *Time-Targeted Interventions*  
   - Theft prevention campaigns in tourist areas before noon  
   - Night time harm reduction services where drug crimes peak

3. *Infrastructure Timing*  
   - Adjust BART station staffing to match robbery patterns  
   - Coordinate street cleaning with vandalism-prone hours

---

### *Storytelling Tips for This Viz*

1. *Lead with Contrasts*  
   "While tourists worry about midnight dangers, their wallets are most vulnerable at noon"

2. *Use Time Metaphors*  
   "The criminal workday begins when yours ends"

3. *Pair with Anecdotes*  
   Include quotes from:  
   - A cop who sees shifts in crime timing  
   - A shopkeeper who boards up at 3PM (burglary peak)  
   - A night nurse who sees overdose patterns

4. *Add Interactive Prompts*  
   "What's happening in your neighborhood at 2AM? Drag the clock to find out"


---

## **Conclusion**

Crime in San Francisco has evolved over the years, with notable declines in certain categories post-2014. However, hotspots remain in high-traffic urban centers. Understanding these patterns helps policymakers and residents address safety concerns more effectively.

**Further Reading:**
- [SFPD Crime Data Dashboard](https://data.sfgov.org/Public-Safety)
- [San Francisco Chronicle: Crime Trends Analysis](https://www.sfchronicle.com)

*(Code and data available on [GitHub](your-repo-link))*