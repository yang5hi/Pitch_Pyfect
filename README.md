# Pitch_Pyfect
Pitch Pyfect Project
Project members:  Staci Wilson, Yang Shi, Zach Moormeier

Background:
	Music is an essential part of our daily life.  Usually, song composition comes from a place of creativity.  In this project, we will approach it from an analytical viewpoint.  Lots of data can be collected about music theory and song structure—for example, key signature, beats per minute, beats per measure, tempo, etc.    
	In this project, we mined through the SpotifyⓇ music database and identified the optimal ranges of these characteristics.  Also, we will search through lyrics by genre in order to identify keywords.

Rationale:
	We want to answer this question: Is there a golden music element ratio to compose a popular song? Do the DNA of the songs agree with the music theory?

Datasets:
We utilized multiple datasets were in this study. On the music theory part, a data set contains 1.2 million tracks were used. The last update on the 1.2 m csv was on 12/20/2020. The contributor first acquired the entire MusicBrainz catalog and then queried the album with UPC (Universal Product Code) and further the tracks information from Spotify API. On the trend study, we used a data set of 175k tracks. The 175k csv dataset was last updated on 01/24/2021, and the contributor searched the SpotifyⓇ API for tracks based on the released year.
Lyrics API cross-check with the SpotifyⓇ  weekly/monthly popular songs. most successful artists by decade

Methods and Findings:
Develop a lyrics keyword search by genre.  Are there specific keywords that show up in the lyrics of pop, country etc.
What are the most popular key signatures songs are composed in?  Are these keys major or minor?
Compare the valence of the different genres.
Analyze tempo/beats per minute
Do explicit lyrics have an effect?
After analyzing the data, are there specific parameters that should be met when composing a pop song, metal song, and country song?


Limitations of the project:
	SpotifyⓇ has over 50 million songs.  We are using a dataset of less than 5% of SpotifyⓇ song library. 
	Geographic limitations 
The definition of ‘popular’ is narrow.
The result can be just as good as the data sample.

Applications:
	Get song recommendations based on listening history.
	Guidelines for composing a commercially successful song

References:

Spotify 1.2M+ Songs


song lyrics dataset

music theory wiki



lyrics from 6 genres
There are two datasets artists-data.csv and lyrics-data.csv, both have data on six musical genres:
Rock
Hip Hop
Pop music
Sertanejo (Basically the Brazilian version of Country Music)
Funk Carioca (Originated 60s US Funk, a completely different genre in Brazil nowadays)
Samba (Typical Brazilian music)
All the data were obtained by scraping the Brazilian website Vagalume using R.

