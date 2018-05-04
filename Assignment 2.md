# Assignment 2

##### By Weijia Li and Zhuo Leng

## Introduction
Highlighted by [Cairo](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/databases-and-reporting-tools/9780133440492), the principle of visualization is to choose the right form of visualisation to encode information and to help the audience extract correct quantitative information from the graph. He proposes a Hierarchy of Elementary, developed and tested by William S. Cleveland and Robert McGill, as a guide to determining the best channels for coding data.

From the Cleverland and McGill, the shape and type of the graphs affects people’s ability to interpret visual encodings and thereby decode information in graphsi.e., their graphical perception. For example, position judgments were more accurate than length judgments and angle judgment; and length judgments are more accurate than area judgments, which in turn are more accurate than volume judgments. However, on the list of [Cleveland and McGill’s](http://www.jstor.org.proxy.uchicago.edu/stable/pdf/2288400.pdf) accuracy list, colour is positioned at the bottom since it provides more generic judgements. [Heer and Bostock](http://delivery.acm.org.proxy.uchicago.edu/10.1145/1760000/1753357/p203-heer.pdf?ip=205.208.116.24&id=1753357&acc=ACTIVE%20SERVICE&key=06A6A3A8AFB87403%2E37E789C11FBE2C91%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1525401382_5051aaaa4a0bd14c059a3780a40c51c9) validated Cleveland and McGill’s results using crowdsourced experiments. 

Such result is counterintuitive since colour has always been a huge component in data visualization and without doubt would influence viewer’s experience when looking at data visualization graphs. There are several roles that colour can play in data visualization. First of all, it can help the viewers to follow the story and compare different attributes across different graphs. Second, colour can also convey a strong message by connecting with the viewer emotionally. For example, red is often used to call out things that the viewers should focus on and grey is likely to be used for things that are not as important. Thirdly, color can communicate with the viewers and deliver the message from the graph more efficiently to the viewers.

Thus, in this paper, we performed an experiment to further investigate past result and to answer the question: to what extent does colour affect graphical perception from heatmap? We hypothesize that with the help of proper color, people will provide more accurate interpretation on the data given within shorter period of time.
## Methods
### Experiment Design
The experiment focus on measuring two key attributes, which are the responding time and answer accuracy. We designed a questionnaire on Qualtrics that is structured in two parts: demographic information and graphic perception test. The demographic questions ask for participants’ age, gender, area of study and highest level of education. We added a screener test to make sure the participants are not color blind. In this way, we can make sure that our data is valid and diverse. The experiment took place on the Amazon Mturk platform, all participants were randomly assigned assigned into two groups after the screening test: the test group and the control group. The control group would be presented with a non-coloured heat map, whereas the test group would read the same map with color on it (presented below). The maps, plot by Tableau software, are visualising top 30 most popular songs played on Spotify in year 2017. The songs are ranked and arranged by the number of streams; a larger area means a larger number of total stream, and thus means a higher rank. Both groups were asked to compare two boxes with a similar area (Despacito featuring Daddy Yankee and Something Just Like This) and to identify the box that represents the song of a larger stream. 

![image](https://user-images.githubusercontent.com/22485624/39613036-1c44afc8-4f2a-11e8-9101-881eb106d7e5.png)

![image](https://user-images.githubusercontent.com/22485624/39613058-3c477b16-4f2a-11e8-8974-a1cbb72d5408.png)

### Data Collection

The questionnaire is linked to Amazon MTurk to collect valid information. To exclude participants who ‘guess answers’, we removed those whose total time of response is less than 30 seconds. 

We posted task at 10:00 pm CST with a request of 200 of assignments. The task is completed in 3.5 hours; the average time spend per assignment is 1 minutes 21 seconds; 202 surveys are collected yet 17 of them are invalid. In the rest of 185 survey samples, 90 participants are assigned into the colored group, and 95 participants are in uncolored group. 44.2% of the participants are between 23 to 30 years old and has a bachelor degree as the highest education level. Among the total population, 26.52% of them majored in engineering and 21.55% did business. By plotting the geographic data provided by Amazon MTurk, most of the participants are located in the US or India.

![image](https://user-images.githubusercontent.com/22485624/39613078-657db84c-4f2a-11e8-8424-58fee6207b65.png)


## Result 
We exam our hypothesis in two dimensions: compare the response time of two groups and compare the accuracy of two groups. 

The density plot of response time is shown below. The density of monochrome group and that of colour group does not show significant different distribution. The p-value from a two sample t-test with different variance is 0.67, meaning there is no evidence show the response time of two groups are different.

![image](https://user-images.githubusercontent.com/22485624/39613095-89a3e19c-4f2a-11e8-9e9a-028ed1ef7f9f.png)

The distribution of answers of the two groups are presented below. The correct answer is to choose Despacito (Featuring Daddy Yankee) to be the one with a larger stream. It is obvious that the accuracy of the coloured group is better than that of uncoloured group: 33.68% of uncolored group and 54.44% of colored group chose the right song correctly. Most participants in uncolored group believe the number of streams of these two songs are the same. 

![image](https://user-images.githubusercontent.com/22485624/39613142-e0f78340-4f2a-11e8-90ec-ec464e81a1aa.png)

![image](https://user-images.githubusercontent.com/22485624/39613154-ec93d17c-4f2a-11e8-9fec-5126f392efd9.png)

 ## Conclusion
Based on the data we collected, participants with the colored graph have significantly higher accuracy rate. However, both the color group and uncolar group have similar response time. As a result, our experiment does indicate that colouring helps people’s graphical perception, but more sophisticated testing is required to determine whether using colours can reduce the participant’s response time.  

There are three limitations: 

1. The sample size is not representative. Due to time and funding constraint, only 185 valid data is collected. A larger sample population may speaks for a different result.
2. No penalty for wrong answer, thus the participants have no incentive to spend time to choose the right answer. This may be the reason of the fact that the response time between the control and testing group show no significant differences.
3. The number of testing questions is limited. Only one group of graphs is included in our questionnaire that we are not able to distinguish whether the answer is under prudent thoughts. Also, the provided testing coloured map is painted in red and orange, there may exists participants who are more sensitive to cold colours than warm colours. The result can be biased.

