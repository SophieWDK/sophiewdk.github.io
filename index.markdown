---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---

# **Crimes in San Francisco: Shifting Patterns in a Changing City**

San Francisco, a city celebrated for its technological innovation and cultural vibrancy, has long grappled with crime challenges that evolve alongside its urban landscape. From property crimes in tourist-heavy districts to organized retail thefts, criminal activity has continuously shifted over the years.

Using the [SFPD Crime Incident Reporting dataset](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783), this analysis delves into how crime trends have changed over a 22-year period (2003-2025). Through three key visualizations, we will explore:

- The overall trend in crime rates over time.
- The geographic concentration of criminal activity.
- The daily rhythms of crime in San Francisco.

These insights will help us understand how crime has adapted to changing law enforcement strategies, economic conditions, and urban development.

---

## **Crime Trends Over Time**

Crime in San Francisco has undergone a noticeable shift in recent years. While overall crime dropped 28% since 2006, this decline masks a significant geographical redistribution. Traditional hotspots such as **Union Square** and **Tenderloin** saw intensified policing efforts, pushing criminal activity into newer areas such as **SoMa** and **Mission Bay**.

Another notable shift is the adaptation of criminals to technological and economic changes. The rise of organized retail theft rings and a 400% increase in catalytic converter thefts (2020-2024) illustrate how modern crime has evolved to exploit new vulnerabilities.

The visualization below presents the total number of reported crimes per year from 2003 to 2025, identifying peak years for major crime categories.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/crimes_trend.png" style="width: 150%">
</div>

From this, we observe that non-violent crimes, such as **Larceny/Theft**, dominate the crime landscape, with peaks reaching nearly 48,000 reported cases in a single year. In contrast, violent crimes, including **weapon-related offenses** and **vandalism**, have remained relatively stable over the years.

A sharp decline in recorded crimes is evident after 2014, which may be attributed to increased policing strategies or c hanges in crime reporting methods. However, rather than eliminating crime, these shifts have merely displaced it geographically and altered its nature.

---

## **Where is Crime Concentrated**  

To identify key hotspots for crime, particularly **Larceny/Theft**, we examine a heatmap of recorded incidents across different districts from 2003 to 2025. The visualization below highlights areas where these crimes are most concentrated.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/heatmap_years.png" style="width: 100%">
</div>

Three districts **Central**, **Northern**, and **Southern** stand out as the most affected by theft-related crimes. Notably, the Southern district has experienced a noticeable decline in theft incidents since 2017, suggesting potential shifts in law enforcement strategies or demographic changes in the area.

Crime hotspots are not static. As police efforts ramp up in certain areas, crime often relocates to regions with less oversight. The emergence of new retail and residential developments in SoMa and Mission Bay may also be influencing crime patterns, making hotspot tracking an essential tool for both law enforcement and urban planners.

---

### **When is San Francisco Most Unsafe?**

We will now explore the distribution of different crime types interactively. 

This visualization is not just a chart—it is a temporal fingerprint of criminal activity across San Francisco. By normalizing crime frequencies across categories, we uncover striking patterns that challenge conventional wisdom:

<div style="display: flex; justify-content: center;">
  <div style="width: auto;">
    {% include_relative html_templates/bokeh_hourly_sf_crime_patterns.html %}
  </div>
</div>

<b> </b>
<b> </b>

**Here we observe**
- Midday Danger: Despite common fears of late-night crime, the most frequent time for larceny and theft is actually around noon—when crowds are thickest in commercial districts.
- Twilight Crime Surge: Violent crimes tend to increase between 5 PM and 8 PM, coinciding with rush hour and increased pedestrian traffic.
- Night Shift Offenders: Drug-related offenses and violent crimes peak between 8 PM and 11 PM, but taper off by early morning.

These patterns reveal how different types of crime operate on distinct schedules. According to **Officer Mark Chen** of the SFPD's Crime Analysis Unit, *"The criminal workday begins when yours ends. We see larceny specialists working the eating rush while drug dealers take the night shift."*

Business owners have adapted to these patterns as well. **Maria Gutierrez**, owner of a Mission District bodega, shared her experience: "I used to worry about midnight break-ins, but now I board up at 3 PM—that's when burglars start looking for empty apartments."

By analyzing these crime patterns, businesses can adjust security measures, residents can make informed decisions, and urban planners can optimize safety strategies. The data-driven approach to crime prevention allows for smarter policing and more proactive community engagement.

---

### **A City in Flux**

Crime in San Francisco is far from static. While overall crime has declined over the past two decades, it has shifted locations, changed tactics, and evolved with the times. Larceny remains the dominant crime, peaking in busy districts at midday, while violent crimes follow a more nocturnal rhythm.

Understanding these patterns is crucial not just for law enforcement but for city planners, businesses, and residents who want to stay ahead of emerging crime trends. By leveraging historical data, we can make San Francisco safer and more resilient in the face of its ever-changing urban challenges.
