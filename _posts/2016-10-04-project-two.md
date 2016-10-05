<center>
<br>
<font face="arial">
<font size="32">Project Two</font>
<br>
Evaluation of the 2000's Top 100 Hits Billboard Data Set


<br>
I started the project by reading in the data with pandas then looking at how the data was stored.  I began cleaning up the data by converting week entries with * to NaN.  I then converted the weeks columns to ints and floats where applicable.  I took the time column and converted it to seconds as an integer.  I converted the artist, track, date entered, date peaked columns from unicode to string to save memory.  Next, I noticed that there were two R&B genres so I combined them.  I left Rock and Rock'n'Roll as separate entities as one could argue that they are two separate genres.
<br><br>
At this point I began exploring the data.  I developed the hypothesis that the longer the track was on the billboard, the higher its average ranking would be.  To test my hypothesis, I calculated the average rank of each track's position on the billboard and added it to the end of my data.  I also counted the total number of weeks each track was on the billboard and added it to the end.  I then created the following graph to show the relation between average song ranking and total number of weeks the track was on the chart.</b>
<br>
<img src="https://jasanford24.github.io/images/billboard_scatter.png">
<br>
I immediately noticed something strange happening at 20 weeks.
<br>
<img src="https://jasanford24.github.io/images/falloff_line.png">
<br><br>
<img src="https://jasanford24.github.io/images/genres_bar.png">
</center>
