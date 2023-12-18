---
layout: home
title: Maslow's Redefinition
subtitle: A Virus Challenging a Staple of Psychology

---
![Maslow_pyramid](assets/img/maslow.jpg)

Maslow's Hierarchy of Needs serves as a model for assessing human behavior, offering insights into the profound shifts witnessed during the pandemic. From altered relationship dynamics to revised safety measures and changing professional priorities, our needs underwent a transformative evolution.

The pivotal consideration lies in whether the data collected during this critical period truly encapsulates our emotions and intuitions. Is it aligned with Maslow's enduring theory, a testament to its continued dominance in shaping our daily lives? This study delves into the pandemic-induced changes, exploring whether Maslow's framework remains a relevant and accurate tool for understanding these shifts.

Our research only encompasses EU countries. By examining the intricacies of the data at hand, we aim to uncover the resonance between our evolving needs and the timeless principles outlined by Maslow's Hierarchy, providing a nuanced perspective on the enduring impact of his theory.
The ultimate goal is to redefine this sacred hierarchy in order for it to resonate with the reality that was the life during the pandemic

This behavioral study bases itself on web-browsing data such as Wikipedia page views and Google trends, transportation and mobility data provided by Google and Apple, and EU-centric unemployment data.

# **Methods**
## Categorization task
While Mobility and Unemployment Data directly point us to the lower-two levels of the pyramid, Physiological Needs and Safety, exctracting data for the upper three levels is a bit more intricate: Wikipedia pages and topics are not intuitively classified into Esteem, Love and Affection and Self-Actualization, this needed to be done in order to complete the study.

## Difference in Differences

# The secrets of the Pyramid
## Physiological Needs

## Safety
EU Unemployment Data revealed a few things about how financial safety's place evolved during the pandemic. Preliminary studies on the overall number of inactive people show how the inactive European population was distributed amongst different groups: the number of inactive men  grew after the lockdown with respect to women, as did the number of unemployed 'young' people (under 25) with respect to 'older ' people (between the ages of 25 and 74). The pie charts help us visualize the results: labels Y_LT25 and Y25-74 respectively represent the younger and older population, as for the M and F labels, they represent male and female individuals. 
 
#### Distribution of Unemployed Individuals per Group
![Unemployment_age](assets/img/un_age.png)
![Unemployment_sex](assets/img/un_sex.png)

Given these results, the next natural step is to generalize to an EU-wide scale, to understand how relevant safety needs related to employment were during covid times, and the answers lie in time-series of unemployment rates across EU countries. Naively, plotting, regressing over the data and extracting coefficients should provide the key elements to infer the evolution of safety needs. 

#### Time-Series of Unemployment Rates per European Country
![C_1](assets/img/country_1.png)
![C_2](assets/img/country_2.png)
![C_3](assets/img/country_3.png)
![C_4](assets/img/country_4.png)
![C_5](assets/img/country_5.png)

Using least squares over this data to estimate the coefficients of unemployment rate change that the lockdown-country interaction brings yield the following results:

![LS](assets/img/ls.png)


This analysis shows that some countries, like Iceland, had a thriving employment situation during lockdown whilst other countries, such as Spain, were struggling with employment levels.
However, it has one main fallacy: it does not take seasonality into account. A fallacy that ***Difference in Differences** solves.

## Love and Belonging

## Esteeem

## Self-Actualizaion
