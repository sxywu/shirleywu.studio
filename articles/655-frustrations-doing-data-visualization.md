---
title: 655 Frustrations Doing Data Visualization
date: 2017-09-21
---

Earlier this year, my friend [Elijah](http://twitter.com/Elijah_Meeks) made a bold claim: that most people in data visualization end up leaving, because there's something wrong with the current state of the field. It stirred quite a bit of conversation, and resulted in a [community survey](https://medium.com/@Elijah_Meeks/2017-data-visualization-survey-results-40688830b9f2) and a [Medium publication](https://medium.com/visualizing-the-field/visualizing-the-field-finding-our-way-6330d3e48555). The survey itself had 45 questions, and ranged from asking for demographic information to the role of data visualization in the respondent's job. It garnered 981 responses, and out of curiosity, I decided to dig into their answers.

Since none of the [survey questions](https://github.com/emeeks/data_visualization_survey/blob/master/data/questions.txt) could actually measure whether people are leaving the field, I focused instead on their frustrations. I wanted to know whether more or less people had frustrations, and how that number correlated with other aspects of their data visualization jobs: if they were hired to do data visualization, were they more likely to have frustrations? What about if they were paid more or less than their UI and design counterparts, or if they worked collaboratively or subordinately with their stakeholders? By looking at the frustrations that come from specific parts of their jobs, I'm hoping to identify the areas that we as a community can work to better.

## A visualization of the visualization community

(I know --- meta, right?)

First things first, here's how to read the visualization (And [here](http://sxywu.com/community)'s where you can play with it):

<div class='images center'>
  <img src="https://miro.medium.com/max/1418/1*TbqvVjcTLVaneKzeE6r9Hw.png" alt="">
</div>

It's made up of dots, each dot representing a survey response. The dots are arranged horizontally by percent of day the respondent spends working on data visualization, and colored by the same metric. It's split vertically by whether the respondent answered the question, *"What is your biggest frustration doing data visualization?"* And there's also a box-plot to show the median and quadrants, so that I can see at a glance if those who responded with frustrations work on data visualization for more parts of their day (in the above, they do).

At any given time, I can choose another set of questions from the survey to look at the spread of their answers. The motivation is to compare two questions and see if there are any correlations.

<div class='images center'>
  <img src="https://miro.medium.com/max/1425/1*i3orvGp9xhs7GpYZlW9EPA.gif" alt="">
</div>

In particular, I decided to explore what factors contribute to more or less time spent working on data visualizations, and what factors to higher or lower (perceived) salaries.

## Those on separate visualization teams spend more time visualizing than those on embedded teams

<div class='images left two'>
  <img src="https://miro.medium.com/max/1210/1*cHYvxTs3BODfWJhakCH_UQ.png" alt="">
  <img src="https://miro.medium.com/max/1224/1*EbumoWy6h-sp0qMV4e1Myw.png" alt="">
</div>

<div class="imagenote up-arrow right-arrow">
  "Were you hired to do data visualization only?" (top left), "Are data visualization specialists represented in the leadership of your organization?" (top right), and "Is there a separate group that does data visualizations or are you embedded in another group?" (bottom).
</div>

<p>
  <img class='left' src="https://miro.medium.com/max/1182/1*D4azQWdyOnVkxls_kadUdw.png" alt="">
  When I started looking at percent of day spent on visualizations, I was expecting some of the results: it makes sense that those hired to do data visualization would work much more on it, and so would those with more representation in leadership.
  <br /><br />
  But what I didn't expect at all: those in a separate visualization group also tend to work on visualizations more than those embedded in another team. I had thought that being embedded in a team --- especially teams working on specific problems or parts of the product --- would mean more chances to work on related visualizations. But in retrospect, it makes sense that dedicated visualization teams --- who get visualization requests from other teams, presumably with datasets already at the ready --- would end up spending more time on creating the actual visuals.
</p>

## Those who focus primarily on visualizations perceive higher total compensation relative to their peers

<div class="imagenote right-arrow">
  "Is your total compensation in-line with Software Engineers and UX/UI/Designer roles at your level?"
</div>

<p>
  <img class='left' src="https://miro.medium.com/max/572/1*E9EbpHGmHjPuu63Sxj-ifA.png" alt="">
  Out of the 981 respondents, only 464 responded that they perceived their compensation to be higher, similar, or lower than other tangential roles; most others responded either that they didn't know, didn't feel comfortable sharing, or didn't respond all together.
  <br /><br />
  And out of those 464, only 82 people (17.6%) responded higher as compared to 179 (38.6%) lower. That's more than twice the amount of people that felt their total compensation was lower!
</p>

So can we find some trends of what might correlate with lower perceived compensation?

<div class='images left two'>
  <img src="https://miro.medium.com/max/2398/1*g3M7HPsKt5VV4r6BCB4XYA.png" alt="">
  <img src="https://miro.medium.com/max/2400/1*X_BMMcihPujb0ENuVVqdqQ.png" alt="">
</div>

<div class="imagenote up-arrow">
Total compensation as filtered by data visualization as a primary focus (left) vs. as one of several (right).
</div>

First interesting observation: of the 82 people that responded a higher perceived compensation, 41% do data visualization as their primary focus, and 21% do it as one of several things. And of the 179 people that responded a lower perceived compensation, the reverse is true; only 21% do data visualization as their primary focus, and 36% do it as one of several things.

<div class='images left two'>
  <img src="https://miro.medium.com/max/1248/1*iDZteJyPH89ZzhVf8z30zg.png" alt="">
  <img src="https://miro.medium.com/max/1232/1*qFsNBpOCC2G6_4USqf8ulA.png" alt="">
</div>

<div class="imagenote up-arrow">
  Total compensation as filtered by a collaborative relationship with the consumer (left) vs. subordinate (right).
</div>

Relationship matters too --- when we filter by a collaborative relationship with the stakeholder, there are more who responded that they perceived higher total compensation than lower. And the opposite is true for a subordinate relationship, a higher percentage of respondents perceive they had lower total compensation.
<br /><br />
So after all the work figuring out the factors leading to less time spent on visualizations, and lower perceived salaries, I decided to filter the respondents by them. I think of this group as the most dissatisfied data visualization practitioners, the ones who are:

- On an embedded team,
- Not hired to work on data visualization,
- Does data visualization as only one of several tasks, and
- Has a subordinate relationship with the stakeholder of their visualization.

And when I looked into their frustrations, I noticed that they fell into two primary categories: those stemming from others in the organization, and those from the technology.

## "Coworkers do not understand what is possible"

The most common frustration that data visualization practitioners cite is the lack of time, often stemming from the organizational lack of respect paid to data visualization:

> One of our senior executives doesn't appreciate data viz and considers herself a "spreadsheet person." So I am discouraged from having fun with viz and extending beyond the basics.
>
> The number of managers that ignore the data because their gut has gotten them this far.
>
> Not enough time for data viz. Data Science/Engineer colleagues do not see the value of it

But other times, it's just because more of the time was taken up by work upstream, with data preparation and exploration:

> It's the last step and therefore gets the least amount of time. Most time is in data exploration.Time crunch because they get the data to you right before the final product is due leaving no time for my work.

But either way, these frustrations stem from a lack of understanding by others in the organization, non-data visualization peers and leadership alike:

> Lack of understanding from supervisors as to the extent of the data prep process and how long it can take.
>
> Coworkers do not understand what is possible
>
> Not included in the initial design of the whole project [...] also goals are vague.

## Difficult data and too many tools

The second most common frustration is having to deal with inconsistent data that are time-consuming to clean:

> Inconsistencies in data quality/integrity produced by colleagues necessitate extensive cleanup and thwarts implementation of automated visualization processes.
>
> Incredible amount of data cleanup work reduces time spent on statistical modeling and visualization design.

Then, once the data is ready, there is also the pain of tooling:

> no general easy access flexible and interactive tools
>
> Too many libraries to work with
>
> Lack of components in some of the BI tools

These are only a few of the frustrations articulated by dissatisfied practitioners, and I have compiled the rest [here](https://docs.google.com/document/d/1jrXjwUqPKenfSqVw5VAsrwXJxM0ZPTpbVQ3xnt2NUi0/edit?usp=sharing).

I'm convinced that with the lack of understanding from leadership and peers, we need to educate on how effective visualizations can benefit them, and what it takes to build those effective visualizations.

These efforts are already undergoing: in [Moritz's essay earlier this year](https://medium.com/visualizing-the-field/there-be-dragons-dataviz-in-the-industry-652e712394a0), he called for more case studies on successful experiences building visualizations for industry. I know that he is [working on one](http://www.nand.io/projects/peak-spotting/). And with [Kim Rees's move to Capital One](https://medium.com/capitalonedesign/launching-data-visualization-at-capital-one-53fa763a8f64), and Uber and Netflix's already-strong visualization teams, we know that many big companies already have data visualizations as a business priority. As more successful case studies emerge from them, I hope more companies will see the value of data visualizations.

But it's not enough for companies to realize that they *want* more visualizations in their practice. They need to prioritize and understand what it takes to build *effective* visualizations, and how to empower those working on them. There's a world of difference between thoughtless charts and graphs with data slapped in, and a full data visualization solution built with the business in mind. The latter requires involving a data visualization practitioner from the very beginning. We need to be briefed on the business use case or problem statement, so we know what to prioritize communicating. We need to work closely with the data, so we know what the data looks like and what the edge cases may be. We need to have a feedback loop with our stakeholders, so we can prototype and iterate --- because the first design is very rarely the right one.

This process requires a broad spectrum of skills, from data engineering and analysis, to design and user research, to prototyping and implementation. I've never met a single person who was strong in every aspect; it's important to recognize where our strengths lay, and to fill our weaknesses either by hiring someone of complementary skills or by allocating more time for where we are weaker.

And finally, we as practitioners need continuous education. I am increasingly convinced that tools like D3 belong in every front-end developer's repertoire, and that our value-add will be in design and prototyping. Few of us had the luxury of studying data visualization, or information visualization, or even HCI design in school, so [books on the subject](https://www.visualcinnamon.com/resources/learning-data-visualization/books) really help. It's also important to keep an eye out for what works and what doesn't work about any piece of data visualization; there are [many](http://flowingdata.com/most-recent/) [newsletters](https://www.dashingd3js.com/data-visualization-and-d3-newsletter) and [resources](http://www.visualisingdata.com/) for that purpose. And when it comes to keeping our toolset sharp --- whether D3, ggplot, or matplotlib --- there are some [great online communities](https://medium.com/@enjalot/the-hitchhikers-guide-to-d3-js-a8552174733a).

I realize that we will always have some frustrations --- but I'm also excited to see what our young community will do with all of this data, and where we'll take this very fresh field of data visualization.

## A post-script

<div class='images center'>
  <img src="https://miro.medium.com/max/1168/1*eoC6CkVUi9_S8ml2ytjaTA.png" alt="">
</div>

I just want to know, those that replied <5% time spent on visualization, but also answered that it was their primary focus...how does that even 🤔?

_Thank you _[_Elijah_](http://twitter.com/elijah_meeks)_ for the constant prodding and encouragement, and _[_Irene_](https://twitter.com/ireneros)_, _[_Nadieh_](https://twitter.com/nadiehbremer)_, _[_Eric_](https://twitter.com/ericsoco)_, _[_Kyle_](https://twitter.com/kyleshevlin)_, and _[_Moritz_](https://twitter.com/moritz_stefaner)_ for the feedback and editing on this piece. Please let me know any feedback and thoughts you have on this data!_
