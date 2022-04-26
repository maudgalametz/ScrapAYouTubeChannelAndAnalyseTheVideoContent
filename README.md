# Scrap a You Tube channel and analyse the video and comments content


### Tools used and installation


- The script uses YouTube API or Selenium to retrieve data out of YT webpages. 
To run the scripts, you will need to also install several Python libraries, including :
numpy, pandas, sklearn, nltk, spacy, ggplot.

To install a package with pip, type:
``` 
pip install my_package
```

*Remarks :* You need to have a working YT API key to run the first notebook.
You also need the yt_stats.py script (and potentially the ngramfreq.py script for the 
future language recognition function).


### Organisation of the notebooks

- 1-ScrapTheChannel.ipynb : 
This notebook retrieves general statistics on the YouTube channel and isolates videos of one month you selected.
We perform a study on how videos comments, likes and views correlate and build a tag word cloud 
of the videos (based on YouTube tags). We finally save independantly the videoIds for future use.

- 2-StudyOneVideo.ipynb : 
This notebook focuses on the most watched video of the month previously selected. 
We isolate its comments, built a word cloud of them, analyse the way their 
associated likes and the feeling expressed within the comments correlate.
We finally perform a quick Latent Dirichlet Allocation topic extraction.

- 3-CommentsSectionTopicExtraction.ipynb :
This notebook analyses all of the videos comments. It performs a LDA topic extraction and build an intertopic distance map.



### To be improved

- Continue investigating the language recognition on the comments to analyse separately non-french commentaries.

- Test other 'feeling' scoring metrics. The one we use is mis-scoring some comments when complex. 


## Versioning

We use python 3.7 


## Authors

Maud Galametz
