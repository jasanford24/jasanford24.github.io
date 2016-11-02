<center>
<br>
<font face="arial">
<font size="32">Project Six</font>
<br><br>
Evaluation of IMDB Top 250 Movie Data

<br><br>
Key Assumptions:
<br> 1) 
<br> 2) 
<br> 3) 
<br><br>


<br>
My model has ~63% accuracy accurately predicting a movies rating to be above or below the median rating, 8.3. My model performs best when trying to predict ratings of recently released films.
I took the top 250 movies off of IMDB and created a model predicting whether a movie was above or below the median rating of the 250 movies. Dropping nulls put the total count down to 246 movies. I Count Vectorized 'Writers', 'Directors', 'Actors', 'Genres', and 'Country'; and I included 'Year', 'imdbRating', 'imdbVotes', and 'Runtime'. I did not include 'Awards' in my model as doing so would prevent my model from being able to accurately model recently released films. I also didn't include Metascore since Metascore is pretty much what I'm trying to predict but labeled under a different metric. I then created two different sets, one with limited features and one with all features. I also used Eigan Vectors to reduce both sets of features in two additional sets. I then ran Extra Trees and Random Forest on the select feature set, full feature set, and select/full bucket sets. I found that 'Extra Trees Default Select Feature Accuracy' and 'Random Forest Default Select Feature Accuracy' were the two most accurate models with minimal difference between the two. With random chance being around 51% for this dataset, my model makes 10-15% more accurate predictions at ~63% accuracy. The top five features with highest importance are 'imdbVotes', 'Year', 'Runtime', 'Country: uk', and 'Genre: adventure'.
With more time, I could emplement additional feature categories to make the model more accurate. I also need to figure out why adding more features decreases the accuracy. My model use to be ~5% more accurate until I changed stuff and messed around. So if I had more time I'd fix that too.
<br>

<br>

<br>

<br>

<br>

<br>

<br>
