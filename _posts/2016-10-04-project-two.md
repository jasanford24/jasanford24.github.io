<center>
<br>
<font face="arial">
<font size="32">Project Two</font>
<br><br>
Evaluation of the 2000's Top 100 Hits Billboard Data Set

<br>
<br>
I started the project by reading in the data with pandas then looking at how the data was stored.  I began cleaning up the data by converting week entries with * to NaN.  I then converted the weeks columns to ints and floats where applicable.  I took the time column and converted it to seconds as an integer.  I converted the artist, track, date entered, date peaked columns from unicode to string to save memory.  Next, I noticed that there were two R&B genres so I combined them.  I left Rock and Rock'n'Roll as separate entities as one could argue that they are two separate genres.  I discovered later that I needed to rename the first ten weeks columns as the pivot_table function tried sorting them alphabetically and it began to throw off my data.
<br><br>
At this point I began exploring the data.  I developed the hypothesis that the longer the track was on the billboard, the higher its average ranking would be.  To test my hypothesis, I calculated the average rank of each track's position on the billboard and added it to the end of my data.  I also counted the total number of weeks each track was on the billboard and added it to the end.  I then created the following graph to show the relation between average song ranking and total number of weeks the track was on the chart.  I inverted the Y-axis to properly simulate the rankings of the billboard chart.
<br>
<img src="https://jasanford24.github.io/images/billboard_scatter.png">
<br>
I immediately noticed something strange happening around 20 weeks.  So I created a graph to depict the decrease in number of tracks as the number of weeks the track was on the billboard increased.  Eighty-one tracks failed to make it from week 19 to 20.  Almost 25% of all tracks stopped at 19 weeks on the billboard.  I found the average of the average ranking of tracks that made it past week 20 and compared it to the average of the average ranking of tracks up to and including week 20.  The rank average above week 20 was 28 while the rank average below week 20 was 69.7.  
<br>
<img src="https://jasanford24.github.io/images/falloff_line.png">
<br>
I decided to look at the genre composite of the tracks that were on the Top 100 Chart for over 20 weeks.  Both Rock and Rock'n'Roll dominated the list.
<br>
<img src="https://jasanford24.github.io/images/genres_bar.png">
</center>
