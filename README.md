# Data Storytelling--EDA of Song Lyrics
### A "data story" on the songs of our times

<img src="figs/title1.jpeg" width="600">

+ This project is conducted by Young Sim
+ **Objectives**: The goal of this project is to look deeper into the patterns and characteristics of different types of song lyrics. Applying tools from natural language processing, interesting findings are derived in this collection of song lyrics.
+ **Summary**: Has it happened to you when a song was really speaking to you? Do you like some of your favorite songs for their lyrics? When you think of a particular music genre (e.g., classic rock), do you expect certain topics for the lyrics? This project conducts exploratory data analysis and topic analysis of song lyrics and find interesting findings and trends over different genres and decades from them. 

  + Data Overview
  <img src="/figs/count_by_genre.png?raw=true" width="600">
  
  There are 10 different genres included in the data. 'Rock' is the most dominant in terms of number of songs. 'Pop', 'Metal', 'Hip-Hop', and 'Country' follow respectively.
  
  <img src="/figs/count_by_decade.png?raw=true" width="600">
  
  Data span from the 1970s to the 2010s. 'Rock' is the most dominant over the whole time period but since 1990s, 'Pop' and 'Hip-Hop' has continued to grow while the proportion of 'Rock' has decreased.
  
  + TF-IDF
       + By Genre        
         
         <img src="/figs/tfidf_metal.png?raw=true" width="500">
         <img src="/figs/tfidf_hiphop.png?raw=true" width="500">
         
       It is notable that 'love' is a common topic over different genres. Meanwhile, 'Metal' and 'Hip-Hop' were the only two genres that the top features did not include 'love'. 'Metal' included words like 'life' and 'time' and 'Hip-Hop' was the only genre with a slang included in top features.
       + By Decade
         
         <img src="/figs/tfidf_1970.png?raw=true" width="500">
         <img src="/figs/tfidf_2010.png?raw=true" width="500">
   
       Top features in different decades were relatively more similar. As in scores by genre, 'love' was a popular word in all times.
   
  + Word Clouds
       + By Genre
       
          <img src="/figs/wordcloud_pop.png?raw=true" width="600">
          <img src="/figs/wordcloud_rnb.png?raw=true" width="600">
          <img src="/figs/wordcloud_jazz.png?raw=true" width="600">
          
       Again, 'love' was a popular word in most genres. An interesting observation on 'pop' is that it talks relatively less about 'love' compared to most other genres except 'Rock' and 'Hop-Hop'. 
       + By Decade
       
           <img src="/figs/wordcloud_1970.png?raw=true" width="600">
           <img src="/figs/wordcloud_2010.png?raw=true" width="600">
    
       The word clouds for different decades were relatively more similar over time. Some popular words of all time include 'love', 'time', 'day', and 'know'.

  + Latent Dirichlet Allocation (LDA)
      + By Genre: Some observations showed similar patterens as in the TF-IDF scores and word clouds. 'Love' was a popular topic among all genres, slangs were included in 'Hip-Hop', and many dark, metaphysical topics were inlucded in 'Metal'. There were also some additional interesting findings. 'Money' related topics were included in 'Pop' and 'Hip-Hop'. Another interesting observation is the way in which 'love' is described in different genres. While 'love' was a popular topic over all genres, some genres tended to talk more about 'love' and in different ways. For example, in genres like 'Country', 'Jazz' and 'Indie', the word 'love' was included in more than 4 topics out of 10. The way in which 'love' is described also seemed to differ between genres. For example, while 'love' was included in the same topic with words like 'fuck', 'never', 'noth', 'everyth' in 'Metal', in 'Country' it was included in the same topic with words like 'sweet', 'shile', 'heaven', and 'angel'.
       + By Decade: As observed in the previous analysis, 'love' has been a popular topic over all times. While in 1980s there were 'love' included in notably more topics than in other decades, there were relatively less difference over time in the way in which 'love' is described compared to LDA modeling by Genre. What is interesting is that starting from 1980s, where data for 'Hip-Hop' was first included, one or more slang is included in the topics for every decade and the number of slangs increase as it gets closer to the 2010s. This reflects the growth of 'Hip-Hop' over decade visualized in the graph 'Percentage of Each Genre by Decade.'

+ **Contributions**: 
    + Performed exploratory data analysis of song lyrics from MetroLyrics in order to write a blog of “data story” on trends and findings such as popularity of different genres by decade and popular topics in each genre.
    + Used data visualization tools, TF-IDF scores, word clouds, and Latent Dirichlet Allocation in Python to analyze the corpus of 100,000+ song lyrics.

+ **Keywords: Exploratory Data Analysis, Natural Language Processing, Text Data Analysis, TF-IDF, Word Clouds, Latent Dirichlet Allocation, Topic Analysis, Data Visualization, Data Storytelling, Song Lyrics, Python**


Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── data/ data used in analytics
├── doc/ preprocessing, report, presentation files, and/or final deliverables
├── figs/ figures
└── output/ analysis output, processed datasets, logs, or other processed things.
```

Please see each subfolder for a README file.
