<center>
<br>
<font face="arial">
<font size="32">Project Three</font>
<br><br>
Evaluation of the 2015 Iowa Liquor Sales Dataset


<h2>Problem Statement</h2>
<p>Given 2015 and 2016 Iowa liquor sales data, determine the best locations for a new storefront.</p>

<h2>Risks and Assumptions</h2>
<p>We chose to work with only 10% of the dataset. There were 2.7 million transactions in the entire data and we only worked with 270,000 transactions. There were also several errors in the dataset. We cleaned up the data as extensively as we could but ended up dropping a couple hundred rows that didn't have complete data. We also did not remove any outliers so there could be one stores that heavily skews the data for certain counties.  </p>
<p>
We assumed that the best place to build a new store would be near stores that are performing exceptionally well. Our main assumption here is that location is the main predictor of success for our store, but a store can perform well for several different reasons. </p>

<h2>Data Analysis</h2>
<p>
We wanted to see which stores had the highest sales and where they were located. Des Moines had the two highest performing stores (2633 and 4829) which had total sales of $407,000 and $363,000 respectively.  

</p>

<p>
	In order to better analyze where a good new store location would be, we added in external data from iowa.gov. We brought in city population and county population which we then planned to use to better predict where underserved markets are. 
</p>

<p>
	We created a linear regression model to try to predict where sales would be highest based on 'County', 'State Bottle Retail' and 'Bottles Sold'. We used the 2015 data as our training data to predict what sales would be like in 2016. Below are graphs of how our model compared to 'Actual Sales' and what the residuals looked like.
</p>
<p>
In order to achieve our main goal of determining where the best performing stores are, we plotted the top 10 counties with the highest sales. Taking it one step further we wanted to see what the average sales were per store in those counties. After correcting to show the results per store, we found that sales per store did not vary nearly as much as sales per county. 
</p>

<p>
	Our next step in determining where we should build a new store was to show 'Profit per Store' and show the top 10 counties. We found that Johnson county had the highest profit per store followed by Polk, Scott, Dallas, Woodbury, Cerro Gordo, Dickinson, Howard, Kossuth, and Linn. We then wanted to make sure that we weren't planning on building a store in a county that had very few stores. </p>

<p>
	The top 10 counties with the highest total of stores are Polk (207), Linn (101), Black Hawk (73), Scott (66), Johnson (53), Pottawattamie (53), Dubuque (40), Story (38), Woodbury (38), and Des Moines(21). So while Dallas had the 3rd highest profit per store, we'd be reluctant to build there since they don't have many stores (17). Alternatively, Polk seems like a great place to build a new store since there are already 207 stores and it still has 2nd highest profit per store. If we built the 208th store, we'd expect for their to be a minimal decrease on the profit per store average in the county whereas if we built in Dallas we'd expect a more significant decline.
</p>

