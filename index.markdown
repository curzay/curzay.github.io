---
layout: default
title:  "Sexual offenses in SF"
date:   2023-03-25 16:51:41 +0100
categories: jekyll update
---

San Francisco levels of crime are a public concern for inhabitants and policy makers. According to the published data from the US government, in terms of crimes per square mile, the national median is around 26.8, while in San Francisco is of 938. Within California, the city of San Francisco stands out as one of the most dangerous cities, as the rate in this state is of 83. Economic and human resources are being allocated into reducing these numbers, but many question if the optimization of these resources is being done in the most reasonable way. As data science techniques evolve, they become a powerful tool to identify crime patterns that had previously been ignored. 

For instance, we can analyse the inference of sexual offenses in the city, discovering which are the patterns occurrence throughout the hours of the day, the days of the week and even the locations of the crimes. Indeed, that is what we see in the following image, a polar plot that shows the count of sex offenses that happen at every hour of the day:

<p align="center">
  <img src="/../figures/polarplot.png" alt="Polarplot hours" height="300">
</p>

This figure shows us the high inference of crimes during the night, between 8p.m. and 2a.m., which is a result that we could expect due to the nature of the crime we are looking into. However, this visualization also reveals a surprising peak at 12p.m., which makes us question why sexual offenses are happening at this hour of the day.

To investigate this further, we displayed the crime occurences by hour and day of the week. We aimed to see if there are specific days in which crimes occur around midnight, and in which crimes occur around midday. In the next interactive bar plot, you can play with different combinations of days of the week and see what time sexual offenses are happening every weekday:

<embed
       type="text/html" 
       src="/../figures/bokeh.html"
       width="800"
       height="800"
       >

If you try and select the days of the weekend, you will see that the nights are dangerous (note that midnight on Saturday and Sunday correspond to Friday and Saturday night). However, one might not guard down during the day (see the peak between 11 and 12 am on Thursday)! 

This tool is really powerful, it can tell us what times of each day the number of officers should be increased. With this, data science can help policy makers turn San Francisco into a safer place, as it helps to identify patterns that were previously hidden behind our beliefs (why would we spend money on preventing sexual offenses between 11 and 12 a.m.? Well, apparently it is a need). 

Now we know what times of the day have a higher crime index, but we don't have infinite resources to cover the entire city at these peaks. So... where do we send San Francisco PD? To solve this question, we can also visualize where these crimes are happening. In the map below, you can see a gradient of the occurrence of sexual offenses in the city. 

Moreover, we wanted to expand on this and see what is the reason these crimes are happening there. For this, we have merged the dataset with the locations of some of the most popular bars and nightclubs among San Franciscans. Feel free to click around and find out which are the most dangerous bar areas in the city.

<embed
       type="text/html" 
       src="/../figures/map.html"
       width="700"
       height="400"
       >

We can see a higher incidence in the center of the city, quite close to an area full of establishments. More in detail, we can identify some clubs that are potentially dangerous, as, for example, the ones placed between Turk street and Geary Street or Pops Clubhouse. Finally, this can show us where the crimes are happening and suggest policies to make the city safer.

Lastly, it is important to highlight that the power of visualizations is just as strong as the data allows, and thus San Francisco PD should make sure the data is bulletproof before making decisions based on it. In other words, in these images, we are seeing patterns that seem unrealistic, which could be due to the lack of details by the victim or to SFPD's neglect to record the data properly. For example, it is difficult to think that almost all sexual offenses are happening at 00:00, as shown in the first figure. Probably, police in San Francisco are not recording correctly at which hour they are happening. Similarly, in the map, we can see that the most common area for sexual offenses is around 800 Bryant St., one of the most common police stations in California and probably the site of the crime report and not the location of the crime. Are these inconsistencies creating a bias on how police resources are distributed?

In conclusion, San Francisco Police Department should catch up with the new data science techniques and control the quality of the data they are collecting about crimes. This would allow them to reduce their levels of crime at least closer to the national median and make the city more appealing altogether. 
