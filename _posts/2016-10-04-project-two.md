<center>
<br>
<font size="32"><font face="arial">Project Two</font>
<br>
Evaluation of the 2000's Top 100 Hits Billboard Data Set


<br>
I started the project by reading in the data with pandas then looking at how the data was stored.  I began cleaning up the data by converting week entries with * to NaN.  I then converted the weeks columns to ints and floats where applicable.  I took the time column and converted it to seconds as an integer.  I converted the artist, track, date entered, date peaked columns from unicode to string to save memory.  Next, I noticed that there were two R&B genres so I combined them.  I left Rock and Rock'n'Roll as separate entities as one could argue that they are two separate genres.
<br><br>
At this point I began exploring the data.  I calculated the average rank of each track's position on the billboard and added it to the end of my data.  I also counted the total number of weeks each track was on the billboard and added it to the end.
<br>
<br><b>The following graph shows the relation between average song ranking and number of weeks on the chart.</b>
<br>
<img src="https://jasanford24.github.io/images/billboard_scatter.png">
<br>
<br>
<img src="https://jasanford24.github.io/images/falloff_line.png">
<br><br>
<img src="https://jasanford24.github.io/images/genres_bar.png">
</center>
