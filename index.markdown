---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---

# **Crimes in San Francisco: Shifting Patterns in a Changing City**

San Francisco, a city celebrated for its technological innovation and cultural vibrancy, has long grappled with crime challenges that evolve alongside its urban landscape. From property crimes in tourist-heavy districts to organized retail thefts, criminal activity has continuously shifted over the years.

This analysis uses official crime records from the [San Francisco Police Department](https://www.sanfranciscopolice.org/your-sfpd/crime-data-reports) (SFPD), covering **January 2003 to January 2025** with over 2.5 million incidents. The dataset comes from [SF OpenData](https://datasf.org/opendata/), the city's official data portal, and includes:

- **Crime categories**: Larceny, assault, burglary, drug offens, etc.
- **Temporal data**: Exact dates and times of reports.
- **Location details**: Police district and geographic coordinates.

Taking all this information into account, through three key visualizations, we will explore:

- The overall trend in crime rates over time.
- The geographic concentration of criminal activity.
- The daily rhythms of crime in San Francisco.

These insights will help us understand how crime has adapted to changing law enforcement strategies, economic conditions, and urban development.

## **Crime Trends Over Time**

[comment]: <> (Crime in San Francisco has undergone a noticeable shift in recent years. While overall crime dropped 28% since 2006, this decline masks a significant geographical redistribution. Traditional hotspots such as **Union Square** and **Tenderloin** saw intensified policing efforts, pushing criminal activity into newer areas such as **SoMa** and **Mission Bay**.) 

[comment]: <> (Another notable shift is the adaptation of criminals to technological and economic changes. The rise of organized retail theft rings and a 400% increase in catalytic converter thefts (2020-2024) illustrate how modern crime has evolved to exploit new vulnerabilities.)

The visualization below presents the total number of reported crimes per year from 2003 to 2025, identifying peak years for major crime categories. The y-axes are the crime count and they have different indices.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/crimes_trend.png" style="width: 150%">
</div>

From this, we observe that non-violent crimes, such as **Larceny/Theft**, dominate the crime landscape, with peaks reaching nearly 48,000 reported cases in a single year. In contrast, violent crimes, including **weapon-related offenses** and **vandalism**, have remained relatively stable over the years.

It is worth noticing a huge drop in **vehicle theft** after 2005. According to [this article](https://www.eastbaytimes.com/2007/02/16/car-thefts-decrease-statewide/); "law enforcement officers across the state have employed new technologies to fight car theft." That could be an explanation for the drop and the reason why the drop has been stable since.

Another observation worth noticing is how the corona pandemic in 2020 may have influenced the different kinds of crimes. There is a huge drop in **theft** but a big rice in **burglary** for instance.

A sharp decline in recorded crimes is evident after 2014, which may be attributed to increased policing strategies or changes in crime reporting methods. However, rather than eliminating crime, these shifts have merely displaced it geographically and altered its nature.

---

## **Where is Crime Concentrated**  

To identify key hotspots for crime, particularly **Larceny/Theft**, we examine a heatmap of recorded incidents across different districts from 2003 to 2025. The visualization below highlights areas where these crimes are most concentrated.

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="figures/heatmap_years.png" style="width: 100%">
</div>

Three districts **Central**, **Northern**, and **Southern** stand out as the most affected by theft-related crimes. Notably, the Southern district has experienced a noticeable decline in theft incidents since 2017, suggesting potential shifts in law enforcement strategies or demographic changes in the area. [Another explanation for the drastically decrease in theft could be that in 2015 San Francisco Police Department opened a new Public Safety Building in the district](https://www.sanfranciscopolice.org/stations/southern-station)

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

**Observations from the plot**
- Midday Danger: Despite common fears of late-night crime, the most frequent time for larceny and theft is actually around noon—when crowds are thickest in commercial districts.
- Twilight Crime Surge: Violent crimes tend to increase between 5 PM and 8 PM, coinciding with rush hour and increased pedestrian traffic.
- Night Shift Offenders: Drug-related offens and violent crimes peak between 8 PM and 11 PM, but taper off by early morning.

These patterns reveal how different types of crime operate on distinct schedules. According to a 2024 report from the [San Francisco Police Department Crime Analysis Unit](https://www.sanfranciscopolice.org/sites/default/files/2024-10/SFPD_CrimeReport_Sept2024_20241015.pdf), organized larceny groups tend to target high-traffic areas during midday hours, while violent crimes such as assaults peak during evening hours. [A study by the Public Policy Institute of California](https://www.ppic.org/publication/crime-trends-in-california/?utm_source=chatgpt.com) also confirms that urban crime tends to follow predictable daily patterns, influenced by foot traffic and economic activity.

[Business owners in crime-prone areas have had to adapt](https://nypost.com/2024/12/12/business/safeway-to-shut-down-san-francisco-supermarket-due-to-rampant-theft/?utm_source=chatgpt.com). Many now implement additional security measures during peak crime hours, such as restricting entry in the afternoon or adding security personnel during high-risk evening periods. These adaptations align with the broader trend of businesses taking proactive steps to deter criminal activity.

By analyzing these crime patterns, businesses can adjust security measures, residents can make informed decisions, and urban planners can optimize safety strategies. The data-driven approach to crime prevention allows for smarter policing and more proactive community engagement.

### **A City in Flux**

Crime in San Francisco is far from static. While overall crime has declined over the past two decades, it has shifted locations, changed tactics, and evolved with the times. Larceny remains the dominant crime, peaking in busy districts at midday, while violent crimes follow a more nocturnal rhythm.

Understanding these patterns is crucial not just for law enforcement but for city planners, businesses, and residents who want to stay ahead of emerging crime trends. By leveraging historical data, we can make San Francisco safer and more resilient in the face of its ever-changing urban challenges.

### Behind-The-Scenes Notebook

This webpage is a project built upon extensive research, data analysis, and coding.
Click the following link to explore a detailed interactive notebook that offers a behind-the-scenes look: [View the notebook](https://github.com/SophieWDK/sophiewdk.github.io/blob/main/data_analysis/behind_the_scenes_notebook.ipynb).
