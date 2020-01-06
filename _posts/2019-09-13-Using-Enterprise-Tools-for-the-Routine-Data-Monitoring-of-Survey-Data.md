---
layout: post
title:  "Using Enterprise Tools for the Routine Data Monitoring of Survey Data"
author: "Adam"
---

Research Optimization is about providing research teams with timely high quality data. To do this at RTI, we rely on a number of open source and commercial data processing tools. <a target="_blank" href="https://powerbi.microsoft.com/">Microsoft Power BI</a> is one of these and as well known business intelligence tool and is available to all enterprise Office 365 customers. Despite its wide availability, there are many features that just aren't widely used, or possible widely understood. In the following case study I going to discuss Power BI and how it can be used for monitoring surveys and analyzing survey data.

![The workshop goers](../assets/luke-chesser-JKUTrJ4vK00-unsplash.jpg "Interviewer training")
<span style="font-size: 14px; font-style: italic;">Dashboards like this one can provide survey researcher with real time statistics on the survey status. Photo by Luke Chesser on <a target="_blank" href="https://unsplash.com/s/photos/monitoring?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
</span>

# Case Study
On a recent survey research project in Jamaica we needed to provide real time updates to researchers here at RTI as well as our partners on this project. For the data collection platform we  used Kobo Collect. You can think of this as an enhanced version of <a target="_blank" href="https://opendatakit.org/">Open Data Kit (ODK)</a>. It's Open Data Kit including the Android mobile app and the backend database plus a whole bunch of other things like a web interface to the survey and a really nice web portal for managing the survey and building the forms, and exporting the data. One of the great things about is its API. Now, for those who aren't familiar with the term, API  is an acronym for <a href="https://en.wikipedia.org/wiki/Application_programming_interface" target="_blank">Application Programming Interface</a>. It sounds pretty techy, but all this means is that the designer of the system has provided a way to interact with the system programmatically. In our case, we use the Kobo Toolbox API to pull the survey responses into PowerBI in the form of a comma delimited value (CSV) file. Once the data is "in" PowerBI then we were able to make dashboards, reports and build out data visualizations.

# But wait, there's more
So far, this is all fine and well, but it's not necessarily novel. While it is true that using an API to hook up a survey platform to a Business Intelligence tool offers a lot of advantages over a traditional file based workflow, this is not a new approach. What PowerBI offers over this is the ability to two additional things:

1. *Scheduled Data Refreshes* Using an API to automatically pull in data is great, but to analyze data on an ongoing survey this process needs to happening regularly - as the interviews are completed. This is exactly what PowerBi schedule refreshes are for. When your data source is a web API, it's possible to configure this data source to be refreshed at regular intervals. For us, the interviewers are to send their completed interviews to the server at the end of every day, so we scheduled the data to be pulled from Kobo Toolbox and into PowerBI every night. This ensures that our dashboards reflect the latest data.
2. *Disseminate the analytics through PowerBI subscriptions* For this study, we developed a dashboard that includes our progress meeting quotas for our supported geographical regions and key populations. To make sure that we allocated resources most efficiently, we wanted this information to be disseminated to the team on a daily basis. Knowing that not everyone on the research team will be able to use PowerBI, we set up something in PowerBI called "email subscriptions". This feature allows this survey dashboard to be emailed out to a list of users at predefined intervals. 

# Conclusions
It used to be the case that conducting survey research relied on manual, paper based processes. However, today there a lot of ways to leverage open source and enterprise software together to automate the data management and reporting of survey data. Microsoft PowerBI has come a long way in the last few years.  So, if you are looking to apply real-time analytics to your survey data, look not further than the tools you probably already own.



