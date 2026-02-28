
RECOMMENDATION-SYSTEM

COMPANY: CODTECH IT SOLUTIONS

NAME: ARYA DILIP BHONGALE

INTERN ID:CTIS4921

DOMAIN:MACHINE LEARNING

DURATION:4 WEEKS

MENTOR:NEELA SANTHOSH KUMAR

DESCRIPTION:
The Mood-Based Music Recommendation System is a content-based filtering system developed to recommend songs according to the emotional mood of the user. Instead of relying on user ratings or collaborative behavior, the system uses Spotify audio features such as danceability, energy, valence, acousticness, tempo, loudness, and liveness to determine the emotional characteristics of each song. These audio attributes help in understanding whether a song feels happy, sad, calm, energetic, or romantic. The primary objective of the system is to analyze these musical features and provide relevant song recommendations that match a selected mood.

The system was implemented using Python as the programming language due to its strong support for data analysis and machine learning. Several libraries were used to build the system efficiently. Pandas and NumPy were used for data manipulation and numerical computations. Scikit-learn was used for feature scaling and similarity calculation. Matplotlib and Seaborn were used for visualization of mood distribution and audio feature relationships. These technologies together enabled efficient data preprocessing, similarity modeling, evaluation, and visualization.

The dataset used in this system contains Spotify music metadata and audio features, including columns such as name, album, artist, popularity, danceability, energy, acousticness, valence, tempo, loudness, and mood. Among these, valence represents the positivity of a song, energy indicates intensity, danceability measures rhythmic suitability, and acousticness indicates how acoustic a track is. These features were selected because they directly influence the emotional perception of music. The presence of a mood column in the dataset made it easier to filter songs according to predefined emotional categories.

During implementation, the first step was data preprocessing. Duplicate entries were removed to ensure data consistency, and missing values were handled to avoid computational errors. The mood labels were standardized to maintain uniform formatting. After cleaning, numerical audio features were selected and scaled using StandardScaler. Feature scaling was necessary because the selected attributes had different ranges, and scaling ensured that no single feature dominated the similarity calculation.

To generate recommendations, cosine similarity was applied to the scaled feature matrix. Cosine similarity measures the angle between two feature vectors and determines how similar two songs are based on their audio characteristics. A similarity matrix was created, and for any selected song, the system identifies the most similar songs by sorting similarity scores in descending order. The top N songs with the highest similarity scores are recommended to the user. This approach ensures that recommended songs share similar musical and emotional characteristics.

For evaluation, Precision@K and Recall@K metrics were used. Precision@K measures how many of the top recommended songs are actually relevant to the selected mood, while Recall@K measures how many relevant songs were successfully retrieved from the total available relevant songs. These metrics help assess the effectiveness and accuracy of the recommendation system. Higher precision and recall values indicate better recommendation quality.

Visualization played an important role in understanding the dataset and validating the system. A bar chart was created to show mood distribution across songs. A scatter plot of energy versus valence helped visualize emotional clustering of songs, where high energy and high valence indicated happy or energetic songs, while low values indicated sad songs. Additionally, average feature comparisons across moods helped confirm that the audio features align logically with emotional categories.

This system is categorized as a content-based recommendation system because it relies solely on item features rather than user interaction data. It is suitable for scenarios where user ratings or listening history are unavailable. However, it does not provide deep personalization without user behavior data. In real-world applications, companies like Spotify use more advanced techniques such as deep learning, collaborative filtering, and user behavior modeling in combination with audio feature analysis. The implemented system represents a simplified academic model that demonstrates the core principles of feature-based music recommendation.
