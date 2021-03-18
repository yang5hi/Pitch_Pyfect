# Pitch_Pyfect

## Pitch Pyfect Project
- Project members:  **Staci Wilson, Yang Shi, Zach Moormeier**

**Background:**
	Music is an essential part of our daily life.  Usually, song composition comes from a place of creativity.  In this project, we will approach it from an analytical viewpoint.  Lots of data can be collected about music theory and song structure—for example, key signature, beats per minute, beats per measure, tempo, etc.    
	In this project, we mined through the SpotifyⓇ music database and identified the optimal ranges of these characteristics.  Also, we will search through lyrics by genre in order to identify keywords.

**Rationale:**
	We want to answer this question: Is there a golden music element ratio to compose a popular song? Do the DNA of the songs agree with the music theory?

**Datasets:**
We utilized multiple datasets were in this study. On the music theory part, a data set contains 1.2 million tracks were used. The last update on the 1.2 m csv was on 12/20/2020. The contributor first acquired the entire MusicBrainz catalog and then queried the album with UPC (Universal Product Code) and further the tracks information from Spotify API. On the trend study, we used a data set of 175k tracks. The 175k csv dataset was last updated on 01/24/2021, and the contributor searched the SpotifyⓇ API for tracks based on the released year.
Lyrics API cross-check with the SpotifyⓇ  weekly/monthly popular songs. most successful artists by decade

**Methods and Findings:**
	We first narrow down our genre studies on Rock, Pop, and Hip-Hop music. With the artist lists we have under those three genres, we cross-check the data with the Spotify data in hand to get a final data frame with tracks(songs), artists, genres, mode, key, tempo, valence, year, and lyrics. We then find out the popular keys, common mode, valence value tendencies, temp range for each genre. We plotted the number of songs we have in our study by publication year. With that information, we utilized New York Times API on the article count of keys words 'Rock Music', 'Pop Music', and "Hip Hop" from 1921 to 2020. As for the lyrics, we first gather all the lyrics we have into a data frame, break down each sentence into words and count the occurrences. Due to the limitation of our knowledge, we have to remove certain none characteristic words by hand to come up with a top 10 list for each genre.

	After analyzing the data, here are our finding:

	- **Key Signatures**
		Songs are composed in key signatures. The most commonly used key signatures in Rock and pop are C, G, D, and A.
		Pop and Rock songs are usually composed of a guitar standpoint.  G, C, D, and A are guitar-friendly key signatures
		Hip Hop music has C# as its most used key signature.  Followed by B and F#.  This is very different from Pop and Rock.
		Hip Hop music is composed of a keyboard standpoint.  When using a keyboard/synthesizer, you have more freedom to compose in any key you want.
		Hip-hop music rarely features guitar as an instrument.  Therefore, this genre is not restricted to using G, C, D, and A 
		That is why more #sharp keys show up. (The key of B is also difficult to play on the guitar)
		In Hip-Hop Music, there is more freedom to experiment using different key signatures.
	- ** mode (major or minor)**
		Key signatures will be major or minor
		The majority of pop and rock music is composed in major keys. 
		Major keys are also more guitar-friendly.  When composing from a guitar standpoint, major keys are easier to play in.
		Hip-Hop shows a 55%/ 45% split between major and minor keys 
		Because hip-hop music is composed of a keyboard standpoint, this genre is free to experiment more with major/minor keys.
		Hip-Hop producers don’t have to cater to the guitar players
		This goes along with our previous point:
		In Hip-Hop music, there is more freedom to experiment using different key signatures.
		This graph further proves, hip-hop music also has more freedom when deciding if the key is major or minor.
	- **Tempo**
		Pop and Rock have a similar distribution.  Most songs are between 100 and 150 beats per minute.
		Most of the Hip-Hop songs we studied have a slower tempo.  According to the histogram, most songs lie between the range of 80 to 100 beats per minute.  
		It is easier to rap over a slower tempo, so you can get as many words in as possible. 

	- **Valence**
		Valence measures the positive (happy) tones vs. negative (sad) tones. Valence does not differ much by genre. Rock and Pop are very similar. 
		Hip-Hop does appear to have a higher valence. However, this could be attributed to the lack of data we had for hip-hop (This chart didn’t tell us much)

	- **Beats Per Measure**
		There is no difference between beats per measure. All three genres compose using 4 beats per measure. (This chart didn’t tell us much)

**Why are Pop and Rock similar?**
	We searched for articles about each genre using the NYT API.  Pop and Rock were created around the same time. Pop and Rock have grown and evolved side-by-side.
Hip-Hop emerged later with the birth of technology/digital recording.

**Final Conclusions**
There is no golden formula for composing the perfect song.  However, depending on the genre, there are a couple of tips to keep in mind:
	- For Rock:
		- Recommended Keys: G, C, D, A
		- Major or Minor?:  Major
		- Ideal Tempo: 100-150 bpm
	- For Pop (Pop has slightly more freedom to experiment with key signature than Rock because it is less reliant on the guitar):
		- Recommended Keys: G, C, D, A
		- Major or Minor? Major
		- Ideal Tempo: 100-150 bpm
	- For Hip-Hop
		- Not restricted to any key, free to experiment
		- Major or Minor? Not restricted, free to use either
		- Ideal Tempo: 80-100 bpm

**Limitations of the project:**
	SpotifyⓇ has over 50 million songs.  We are using a dataset of less than 5% of the SpotifyⓇ song library. We are also using the Brazilian website Vagalume. 
	Geographic limitations 
	The definition of ‘popular’ is narrow.
	The result can be just as good as the data sample.

**Applications:**
	- Guidelines for composing a commercially successful song in rock, pop, and hiphop genres.
**References:**
	- [music theory wiki](https://en.wikipedia.org/wiki/Music_theory)
	- [song lyrics from 6 genres](https://www.kaggle.com/neisse/scrapped-lyrics-from-6-genres)
	- [Song lyrics dataset](https://www.kaggle.com/deepshah16/song-lyrics-dataset)
	- [Spotify 1.2M+ Songs](https://www.kaggle.com/rodolfofigueroa/spotify-12m-songs)
	- [Spotify 1921-2020](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks)
	- [NYT API](https://developer.nytimes.com/docs/articlesearch-product/1/overview)
	
	
