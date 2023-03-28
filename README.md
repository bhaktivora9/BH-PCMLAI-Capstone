### Project Title
Auto Tagging / Auto Classify tracks on basis of audio features.

**Author**

  Bhakti Vora

#### Executive summary

#### Rationale

**Music** and **Talk Shows** or **Podcasts** has been an essential aspect of all human civilizations.
Music has power to emotionally, morally, and culturally affect society.
Whereas Podcasts gives you the platform to raise awareness and create real social change, gain knowledge on various topics in-depth.
Over past decaded the borders between music worlds have disappeared, credit goes to globalization.

Given these conditions music streaming apps have seen tremendous rise in content/data.This results into tremendous work load for subject matter experts to classify / categorize tracks on basis of their content.

**This is where AI can help to reduce human effort of auto labelling audio tracks on basis of audio features. This labelling can be further extended to improvise recommending content to users.**

#### Research Question
*Creating a model that can be used to auto classify (categorize multi label) songs on basis of audio features.*

#### Data Sources
> *_NOTE:_*  Spotify open API's used to gather data
> API's used to gather data.
> - GET https://api.spotify.com/v1/browse/categories,
> - GET https://api.spotify.com/v1/browse/categories/{category_id}/playlists
> - GET https://api.spotify.com/v1/playlists/{playlist_id}/tracks
> - GET https://api.spotify.com/v1/audio-features/{id}
#### Features
##### danceability _(float)_
_Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable._

##### energy _(float)_
_Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy._

##### key _(float)_
_The key the track is Integers map to pitches using standard Pitch Class notation. Eg. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no key was detected, the value is -1._

##### loudness _(float)_
_The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db._

##### mode _(float)_
_Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0._

##### speechiness _(float)_
_Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks._

##### acousticness _(float)_
_A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic. acousticness >= 0 acousticness <= 1_

##### instrumentalness _(float)_
_Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0._

##### liveness _(float)_
_Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live._

##### valence _(float)_
_A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry) valence >= 0 valence <= 1_

##### tempo _(float)_
_The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration._

##### categories _(String)_
_'Pop', 'Party', 'Dance/Electronic', 'Rock', 'R&B','At Home' ,'Romance', 'Chill', 'Jazz', 'Workout', 'Hip-Hop', 'Gaming', 'Summer', 'EQUAL', 'Indie', 'Mood','Travel', 'Indian Classical', 'Devotional', 'Wellness','RADAR', 'Classical','Instrumental',  'Sleep', 'Focus', 'Kids & Family','Cooking & Dining', 'Folk & Acoustic', 'Metal'_

#### Methodology
 - Logistic Regression
 - SVM
 - Decision Tree
 - KNN Classification.

#### Results
  - [Initial Analysis and Data Prepration](https://github.com/bhaktivora9/BH-PCMLAI-Capstone/blob/master/notebooks/initialAnalysis.ipynb)

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
 - bhaktivora09@gmail.com
##### Future Scope 
 - Genre Classification.
 - Build a Recommendation System on top of this model, get Users data from spotify.
 - Extend the research for podcasts other regional music etc.
