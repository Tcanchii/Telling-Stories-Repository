| [home page](https://tcanchii.github.io/Telling-Stories-Repository/) | [visualizing debt](visualizing-government-debt) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Gathering and Processing Data

The data I used was census data about the jobs taken by people that graduated college by degree type. I had initially found [this](https://datausa.io/) website where they took that census data and separated it by major and did [data dashboards](https://datausa.io/profile/cip/mathematics) about the relevant statistics. I specifically noticed a pattern where most majors were generally not centralized into one job field after graduation, and so I decided to compile the data for these into one file to do analysis on it to see if that supported my story/hypothesis that most majors do not force a specific job type for graduates. Unfortunately, there are 1837 listed degree types and having to download a csv file for each one and then somehow squeeze all that information into relevant graphics did not seem feasible so I settled with picking 10 of the common degree types that I thought would give a general spread of potential interests. 

After downloading the data, it took some time writing python scripts to get the data first into one [dataset](finaldata.csv) then to also convert it into the [format](flourishData.csv) required by flourish. This was to get the general information set up for use, and I then ran some calculations \(such as standard deviation calculations, mix/max, etc\) on the data to find interesting/useful trends. The only thing that I found particularly interesting was that, as I suspected, the max centralization of a given major in any specific job type was not very high except in rare circumstances. I then turned that info into a flourish readable [dataset](flourishdata2.xlsx) to also use. 

# Wireframes / storyboards
The overall story wireframe is that it is a conversational piece aimed at high schoolers where the goal is to hopefully both be informative and remove some fears about picking a major. Specifically, the story walks through a basic setup of the fears a high schooler might have about getting locked into a specific career path due to their major, gives a naive approach of how they might be thinking to do research on their major, then gives a more broad approach to looking at trends across majors and points out that the data is suggestive of most majors not being particularly locked into a specific job type. It leaves off with a call to action to not worry so much and to just pick something they find interesting with a few supporting strategies if they don't find those actions compelling enough. 

The storyboard uses a very basic color scheme since it is a more informational topic than a topic with an emotional theme, but I do use traval imagery throughout as it is a transitional decision where there is a lot of unknown. I use red to highlight potentially bad things and blue to highlight potentially good things. Mainly the color choices are to highlight the majors that are too specific and the blue to highlight ones that are more general, hopefully making it visually very easy to get a feel for what majors to pick as a high schooler that doesn't know what they want to do long term. 

[Here](https://preview.shorthand.com/ZxdVqTYWLQNiCs2N) is the preview from shorthand.

## The data visualizations

The first is a slightly messy breakdown of the percent of graduates in each job field by major. This is aimed to accomplish 2 ideas: the first is that you can see a broad overview of relative shares of each job field so that you can see roughly how spread out each major is, and the second is that it is still a little messy and can be broken down into something even simpler.
<div class="flourish-embed flourish-chart" data-src="visualisation/15227514"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

The second is a significantly cleaner idea where it just shows the largest share of graduates in one specific job field. This is aimed to be a very clean metric that highlights how most are not super high and that if the maximum is low for all of them, then the spread of them is necessarily pretty high. Presenting the most synthesized, clean graphic last also presents the sub-narrative that you can take complex data and turn it into easily digestable and useful data; something not important to the main story itself but both a way to "calm" things down in tone and provides a reasonably instructive narrative for students.
<div class="flourish-embed flourish-chart" data-src="visualisation/15228767"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


## Target audience
The target audience is high schoolers that are about to apply for colleges. In particular, high schoolers that are stressed out about how big a decision this could be and either don't know what they want to be doing or feel worried that their choice might be a "wrong" choice and that they might accidentally set themselves up to be stuck in a miserable job. Potentially they have parents or other people in their life asking them about what they want to do and just adding to the overall pressure/stress about the decision. 

What the target audience is not are the high schoolers that have a very specific goal in mind of what they want to do for work when they are older and/or have a lot of experience doing something like coding and know that they want to do computer science or something similar. While they are also high schoolers applying for colleges, the core of this story is to help relieve stress about getting stuck with your choice and so if they do not have that fear \(through being deliberately niche or through experience\) then this story is not helpful for them.

## Interview script

The main issue I have is that I feel like I am generally very to the point so my stories might not feel long enough. I also am not the strongest with transitions and have a tendancy for putting words instead of visuals. The goal with the interviews are to address those specific concerns.  

| Goal | Questions to Ask |
|------|------------------|
|to verify that the story feels like an apporpriate length|Does the story seem long enough?|
|to verify that the story feels like an apporpriate length|Is there anything you felt was missing in the story?|
|Transitions are appropriate|Does the presentation flow well, or are there specific choppy parts?|
|Is there enough visuals|Does the presentation feel too wordy?|
|Is there enough visuals|Is there any specific color choice or imagery that feels off?|
|Is there enough visuals|Is there any color choice or imagery that feels missing?|

Due to the timing of it all, I ended up asking two of them first, made some of the easy corrections, then showed it to the third person. 

## Interview findings
I interviewed three of my friends, all of whom are 26-27, two are in the MISM-BIDA program and one in ISPM. I expected the MISM-BIDA friends to give more technical feedback since they are both also in the course. My ISPM friend is from a strong humanities background so I figured they would give stronger feedback on the flow of the story. Below describes the takeaways I got from each person but the interview responses themselves are linked [here](https://docs.google.com/spreadsheets/d/1vEl8c2vpl0JuiZZK9X_Hj496drUW5yt9hZ_jEonpLh8/edit?usp=sharing). The third was done in person and not included. 

| Questions               | Interview 1 (takeaways) | Interview 2 | Interview 3 |
|-------------------------|--------------------------------|-------------|-------------|
| Does the story seem long enough? | Length is dependent on the playing with interactive visuals|good length||
|Is there anything you felt was missing in the story?|There are more concerning topics than type of job field such as expected salaries|provide outside sources||
|Does the presentation flow well, or are there specific choppy parts?|graphs require playing with and the ending is choppy|ending is choppy with too many colors||
|Is there any specific color choice or imagery that feels off?|tone was not effective|too wordy at the start||
|Is there any color choice or imagery that feels missing?|word coloring was mostly a miss|first graph was not effective||

Most of these ideas are actionable but there are a few that are not feasible. The main one that isn't particularly feasible is the inclusion of other topics such as expected salaries for job types. While that data does exist, it tells a completely different stroy where major does matter which would make the analysis too nuanced. The goal is for an audience that is searching for what they want to do independent from the salaries attached, and although this target audience may be admittedly small, it is still a target audience I can aim at with the data I currently have.

# Identified changes for Part III
The most important change is that the first graphic could be split into multiple ones. This serves two major purposes, the first is to make it less visually painful to look at since it can be made into bar graphs instead of a layers. The second, is that most of the length is looking at these specific graphs where splitting them out more deliberately will force the reader to take more time looking through them all.

The next main change is that the colors should be dialed back to more neutral ideas, and the conclusion/call to action should be expanded a little further. Below are the highlighted changes

| Research synthesis                       | Anticipated changes for Part III                                                |
|------------------------------------------|---------------------------------------------------------------------------------|
| First graphic is not effective | Split it into multiple graphs for different majors, remove the year and just do the most recent \(or keep it for the first and note it doesn't change much over time\) and add a story walking through the different ones |
|too much word colors|use word highlights very sparingly, maybe only at the start|
|text over graphics was hard to read sometimes|consider changing some text over graphics to be more readable|
|call to action was abrupt|include some more information about things to do|
|tone was not effective|consider changing tone to be more informative than conversational|

Overall I think these are all actionable changes. The only one I am unsure on is the text over graphics one since I feel as though my imagery is already feeling very sparse. Removing some of the middle text over graphics and include more charts might make the tone less exciting but it definitely makes the topic more digestable. Hopefully I can find a solid middle ground.

For tone I will likely keep it conversational but try and make it just flow a little better as a solution.
