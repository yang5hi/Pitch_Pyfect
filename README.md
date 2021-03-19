# Pitch_Pyfect

## Pitch Pyfect Project
- Project members:  **Staci Wilson, Yang Shi, Zach Moormeier**

**Background:**
	Music is an essential part of our daily life.  Usually, song composition comes from a place of creativity.  In this project, we will approach it from an analytical viewpoint.  Lots of data can be collected about music theory and song structure—for example, key signature, beats per minute, beats per measure, tempo, etc.    
	In this project, we mined through the SpotifyⓇ music database and identified the optimal ranges of these characteristics.

**Rationale:**
	We want to answer thse questions: Is there a golden music element ratio to compose a popular song? Do the DNA of the songs agree with the music theory? Where are those difference come from and why?

**Datasets:**
	We utilized multiple datasets in this study. A data set containing 1.2 million tracks was used. The last update on the 1.2 m csv was on 12/20/2020. The contributor first acquired the entire MusicBrainz catalog and then queried the album with UPC (Universal Product Code).  He combined this data with data from the Spotify API. On the trend study, we used a data set of 175k tracks. The 175k csv dataset was last updated on 01/24/2021, and the contributor searched the SpotifyⓇ API for tracks based on the released year.
Lyrics API cross-check with the SpotifyⓇ  weekly/monthly popular songs. most successful artists by decade

**Methods and Findings:**
	We first narrowed down our genres to Rock, Pop, and Hip-Hop music. With the artist lists we have under those three genres, we cross-checked the data with the Spotify data in hand to get a final data frame with tracks(songs), artists, genres, mode, key, tempo, valence, year, and lyrics. We then find out the popular keys, common mode, valence value tendencies, temp range for each genre. We plotted the number of songs we have in our study by publication year. With that information, we utilized New York Times API on the article count of keys words 'Rock Music', 'Pop Music', and "Hip Hop" from 1921 to 2020. As for the lyrics, we first gather all the lyrics we have into a data frame, break down each sentence into words and count the occurrences. Due to the limitation of our knowledge, we have to remove certain none characteristic words by hand to come up with a top 10 list for each genre.

After analyzing the data, here are our finding:

- **Key Signatures**
	Songs are composed in key signatures. The most commonly used key signatures in Rock and pop are C, G, D, and A.
	Pop and Rock songs are usually composed from a guitar standpoint.  G, C, D, and A are guitar-friendly key signatures
	Hip Hop music has C# as its most used key signature.  Followed by B and F#.  This is very different from Pop and Rock.
	Hip Hop music is composed from a keyboard standpoint.  When using a keyboard/synthesizer, you have more freedom to compose in any key you want.
	Hip-hop music rarely features guitar as an instrument.  Therefore, this genre is not restricted to using G, C, D, and A 
	That is why more #sharp keys show up. (The key of B is also difficult to play on the guitar)
	In Hip-Hop Music, there is more freedom to experiment using different key signatures.
- ** mode (major or minor)**
	Key signatures will be major or minor
	The majority of pop and rock music is composed in major keys. 
	Major keys are also more guitar-friendly. 
	Hip-Hop shows a 55%/ 45% split between major and minor keys 
	Because hip-hop music is composed of a keyboard standpoint, this genre is free to experiment more with major/minor keys.
	Hip-Hop producers don’t have to cater to the guitar players
	This goes along with our previous point:
	In Hip-Hop music, there is more freedom to experiment using different key signatures.
	This graph further proves, hip-hop music also has more freedom when deciding if the key is major or minor.
- **Valence**
	Typically, major key signatures are used to compose happy songs and minor keys are used for sad songs.
	We predicted that songs composed in a major key would have a higher valence and songs composed in a minor key would have a lower valence.
	However, this is not the case
	It is possible to write a happy song in a minor key and vice versa
- **Tempo**
	Pop and Rock have a similar distribution.  Most songs are between 100 and 140 beats per minute.
	Most of the Hip-Hop songs we studied have a slower tempo.  According to the histogram, most songs lie between the range of 80 to 100 beats per minute.  
	It is easier to rap over a slower tempo, so you can get as many words in as possible. 
- **Beats Per Measure**
	There is no difference between beats per measure. All three genres compose using 4 beats per measure. (This chart didn’t tell us much)

**Why are Pop and Rock similar?**
	We searched for articles about each genre using the NYT API.  Pop and Rock were created around the same time. Pop and Rock have grown and evolved side-by-side.
	Hip-Hop emerged later with the birth of technology/digital recording.

**Final Conclusions**
	- If you want to compose a typical rock song, make things easy on yourself and put it in G, C, D, A and make sure the key signature is major.  
	- Optimal tempo = 100-140 bpm
	- For pop, follow the same guidelines but know you have slightly more freedom to experiment with key signature because you are less reliant on guitar
	-For Hip-Hop,  feel free to experiment with any key signature whether it be major or minor
	Pull your tempo back to about 80-100 bpm, so it’s easier to rap over


**Limitations of the project:**
	SpotifyⓇ has over 50 million songs.  We are using a dataset of less than 5% of the SpotifyⓇ song library. 
	We are also using the Brazilian website Vagalume for its genre, lyrics and artist data.
	Geographic limitations 
	The definition of ‘popular’ is narrow.
	The result can be just as good as the data sample.

**Applications:**
	- Guidelines for composing a commercially successful song in rock, pop, and hiphop genres. <br>
	
**References:** <br>
	- [music theory wiki](https://en.wikipedia.org/wiki/Music_theory) <br>
	- [song lyrics from 6 genres](https://www.kaggle.com/neisse/scrapped-lyrics-from-6-genres)  <br>
	- [Song lyrics dataset](https://www.kaggle.com/deepshah16/song-lyrics-dataset)  <br>
	- [Spotify 1.2M+ Songs](https://www.kaggle.com/rodolfofigueroa/spotify-12m-songs)  <br>
	- [Spotify 1921-2020](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks)  <br>
	- [NYT API](https://developer.nytimes.com/docs/articlesearch-product/1/overview)  <br>
	
