# Jump Scare Data Viz Battle for October 2019
Submission for the [monthly data vis battle](https://www.reddit.com/r/dataisbeautiful/comments/dei68x/battle_dataviz_battle_for_the_month_of_october/) from r/dataisbeautiful.

Demo > https://gem0303.github.io/JumpScare-DataVis-Oct2019/

**Month:** October 2019  
**Theme:** Jump Scares

This was my first time doing data visualization and working with D3. I was interested in mapping the IMDB and Jump Scare scores over time.

### Observations
It looks like the average IMDB score trends down over time. However, this might be caused by people only bothering to rate good older movies on IMDB. No one wanted to take the time to go rate bad movies from the 1960 and 70s. I am not familiar enough with the genre to know how many older movies could be missing. It also appears that, while the IMDB scores trended down, jump scare scores increased. 

Note: the original data set had a jump scare range of 0-5. I converted it to 0-10 to match the IMDB score range.

### Problem: Having both data sets on screen at the same time created a lot of dots/data points.
Solution: I created a slider that controlled the opacity of each data set. You can drag the slider to the left to only view IMDB scores, and to the right to only view Jump Scare scores.

### Problem: A lot of dots overlap each other, due to movies being released in the same year that have the same score.
Solution: I lowered the opacity of each dot to make the "dense" patches of dots more clear. I also created a tooltip that shows a list of all movies sharing the same data point on hover.


### Thoughts for my next data-vis project
- Investigate alternate ways to display overlapping data, such as swarmplots. Consider when it's worthwhile to simplify data to a line graph instead of showing all data points.
- The chart is responsive, but the tooltip gets cut off on smaller screens. Figure out a way to orient it to the left of the dot when needed.
- Draw a line/bezier curve between the data point for a movie's IMDB score and its jump scare score. I'm currently highlighting the matching data point, but this doesn't work for dense areas where dots overlap.
