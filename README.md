# Song Popularity Prediction & User Recommendation Engine

# Background


A group project to predict Song Popularity and build a song recommendation engine while also providing a dashboard to present the findings. It is coursework for "Decision Making with Business Intelligence and Analytics" as part of the MS Data Analytics program at Seattle Pacific University.

<br />The presentation of the background information, EDA, and findings can be found on [Google Data Studio](https://datastudio.google.com/reporting/713ae7af-0154-4a7b-9b52-467bbd2e2a72).

### Data Sources

>User data is obtained from [The Echo Nest Taste Profile](http://millionsongdataset.com/tasteprofile/). 
<br />Song data is obtained from [Million Song Dataset Subset](http://millionsongdataset.com/pages/getting-dataset/#subset).
<br />Artist location data is obtained from [Million Song Data Additional Files](http://millionsongdataset.com/sites/default/files/AdditionalFiles/artist_location.txt).
<br />Track genre data is obtained from [tagtraum industries](https://www.tagtraum.com/msd_genre_datasets.html).
<br />Unique tracks data is obtained from [Million Song Dataset Additional Files](http://millionsongdataset.com/sites/default/files/AdditionalFiles/unique_tracks.txt).
<br />Track by year data is obtained from [Million Song Dataset Additional Files](http://millionsongdataset.com/sites/default/files/AdditionalFiles/tracks_per_year.txt).
<br />Python Source Code to read the HDF5 files into a dataframe from a [github repository by tbertinmahieux](https://github.com/tbertinmahieux/MSongsDB).

***The company background:***
<ul>
  <li>A music streaming platform is hoping to see how data can increase revenue and solve their business probelms.
</ul>

***The presented problems:***
<ul>
  <li>The client wants to maximize listening of their most popular songs to increase revenue by promoting these songs to users.</li>
  <li>Provide users with other songs they can listen to and increase revenue by keeping users engaged on the platform. </li>
</ul>

***The presented solutions:***
<ul>
  <li>Build a regression model to predict song popularity, so that popular songs can be identified right away and promoted to users.</li>
  <li>Build a recommendation engine to recommend songs, so that when a user is on the platform suggested songs can keep them actively listening. </li>
</ul>

## Instructions


The python code in the [notebook](https://github.com/Samantha-Britschgi/Song-Popularity-Prediction-User-Recommendation-System/blob/734674d33b066ee7be29803dd46dcb1d44eebf4a/PROJECTCODE.ipynb) and was written inside of Google Colab, but any editor or IDE that utilizes python will work.  

## Process


 ><ol>
> <li>Changing the Python Source Code from Python 2 to Python 3</li> 
>   <li>Installing & Importing Libraries</li>
>    <li>Data Wrangling
>    <ol>
 >     <li>Creating two dataframes (one for each model) by merging multiple datasets</li>
 >     <li>Removing null values</li>
>      <li>Creating new variables for the song popularity prediction model</li>
>    </ol>
>    </li>
>    <li>Exploratory Analysis using Plotly</li>
>    <li>Model Building & Model Analysis</li>
>      <ol>
><li>Song populatiry prediction model</li>
><li>User recommendation engine model</li> 
></ol>
></li>
>    <li>Recommendations & Next Steps</li>
></ol>

## Models



### ***Song Populatiry Prediction Model***

   <img src="https://github.com/Samantha-Britschgi/Song-Popularity-Prediction-User-Recommendation-System/blob/68123e0cb4e2f6413de6d6df33c4c44b3e2cd5a8/Images/SongRegressionModelSteps.png" width="550" height="300" />


### ***User Recommendation Engine Model***

   <img src="https://github.com/Samantha-Britschgi/Song-Popularity-Prediction-User-Recommendation-System/blob/68123e0cb4e2f6413de6d6df33c4c44b3e2cd5a8/Images/UserRecommendationEngine.png" width="550" height="300" />

## Findings


### ***Song Popularity Prediction Model***

<ul>
<li> Artist Familiarity & Artist Hotness/Popularity are important factors to predict song popularity.</li> 
<li> It is recommended that promoted songs come from artist that have a large fan base and are more well known across the population.</li> 
</ul>

### ***User Recommendation Engine***

<ul>
<li> Content-Based Filtering was done as it recommends what a user will like based on what that user has liked in the past. </li> 
<li> Genre & year were more prominent variables than location of the artist when recommending songs.</li> 
</ul>

## Shortcomings


<ul>
<li>Song Popularity Prediction Model only had a subset of data, ideally it would have more data (especially song energies & song danceability). </li> 
<li>Majority of music within data subset was released between 1990 - 2010 so more data to include current artists would create more accurate recommendations.</li> 
<li>User recommendation engine is only effective for users who have listened to songs on the platform before. </li> 
</ul>
