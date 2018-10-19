---

layout: post
description: datafest 2018
---



<h2>datafest 2018</h2>
<h3> runner up: best analysis</h3>

<br/> 

<img src="/img/datafest.jpg" height="400" class="col one left">

I participated in ASA DataFest 2018 on a team along with Travers Parsons-Grayson, Amanda McFarland, Sam Weiner, and Eli Schwamm. For some background, DataFest is basically a hackathon but instead of development skills we practice our data crunching skills. Each year, they provide us with an industry dataset of millions of rows, as well as 72 hours to do what we can with it. This year, it was Indeed data on job searches. This included data on clicks by users of the site.

<br/>

My friends and I were interested in analyzing the data in ways that could be utilized for public good. Aware of the growing urban-suburban divide and the spatial mismatch hypothesis, we wanted to explore whether people searched for jobs near where they lived. So, we decided to explore the following: <b> Are differences reflected in job search in cities versus suburbs? Do jobs posted in cities and suburbs differ in their proportion of clicks that are local?</b>

<br/> 

We categorized locations into cities and suburbs designated by the Census Bureau. We performed our analysis by testing the hypothesis that the proportion of local clicks in the city was the same as the proportion of local clicks in the suburbs. We also ran a linear regression with city density and metropolitan area fixed effects, on a subset of the data. 

<img src="/img/datafestplot.png" width="620" class="col two right">

In the image to your right, you can see that there is a lower proportion of local clicks for jobs that require higher education versus those that require only a high school diploma. Likewise, there is a higher proportion of local clicks for jobs that are in the city versus those that are located in the suburbs. Through hypothesis testing, we showed that the difference in proportion of local clicks for cities versus suburbs is significant across education groups. 

<br/>

We also constructed maps by education level of proportion of local clicks in each suburb. You can see here, in maps of New York City, that bigger circles exist in blue than in red-- representing higher proportions of local clicks for lower-education jobs. We can also see in both maps that circles are bigger in the center of the city compared to the suburbs-- representing the higher proportion of local clicks for jobs in the city. 

<div class="img_row">
	<img class="w3-half-padding" src="/img/nychs.png">
	<img class="w3-half-padding" src="/img/nychighered.png">
</div>


<br/>

We found that jobs posted in cities attract a significantly higher proportion of local interest than do jobs in the suburbs. This is perhaps related to the national government's investment in highways and automobile transport. To find out more about what we did, read our <a href="{{ site.baseurl }}/DataFest2018PPT.pdf">PowerPoint</a> or our <a href="{{ site.baseurl }}/DataFest2018Writeup.pdf">write-up</a>.