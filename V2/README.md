# UdacityD3 - D3 learning project

## Summary

My visualisaztion was designed to look into the effect of clock time on chance creation in mens Soccer, I also wanted to see whether any changes were uniform across shot types.  The data was scraped as a text commentary and parsed into a data file containing minute, shot location, shot type & outcome. A probit model was then fitted to assign a value to each shot.

### Design

Originally I first plotted a line graph with no facet for type, however this hid many different stories.
I then changed the plot to a scatter plot with the colour of the dots indicating type of shot.

### Feedback

Person 1. Difficult to see data values for individual point.

Person 2. Large range in y values makes plot appear zoomed out.

Person 3. Plot looks basic.
          Legend not in same order as points on plot.

### Edit

In response to the feedback I made a few changes;
1.  I added a tool tip which highlights the data values for a point when hovered over.
2.  I added zoom & drag functionality to the graph so a user can look into specific time periods/points.
3.  I added grid lines, reduced the opacity of the points, moved the legend to the top right of the plot & changed the legend icons to circles to match the plot.
4.  I could not figure out how to re-order the legend.

### Improvements

1.  I scraped my data using R, and used dplyr there to aggregate my data into totals for individual minutes (Look into using roll-up to aggregate data using D3). This is now added in v2.
2.  Add buttons so the user can choose which type of shot they want to look at.
3.  Add animation to plot the points in time order with a line of best fit following.
4.  Add something to indicate half time at 45 minutes, resulting in low numbers for minute 45. This is now added in v2 with 2nd y axis showing half time.
5.  Add a way of displaying injury time data. (This was removed from my data file due to all injury time being labelled as either minute 45 or 90, regardless of how many minutes were played).
6.  In v2 zoom & drag functionality was removed due to it not really being necessary, data & legend are now ordered in the same way & a subtitle has been added.

### Resources

I looked through several different visualations and took ideas from a few to create this visualisation, most notably from below.
http://bl.ocks.org/mbostock
https://github.com/d3/d3/wiki/Gallery

