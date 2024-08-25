# Media-Bias-Detector

This detector will be heavily influenced by https://medium.com/@danilo.najkov/detecting-political-bias-in-online-articles-using-nlp-and-classification-models-c1a40ec3989b. However this seems to have used Russian news sites for data, I will be scraping data from sites following https://www.allsides.com/media-bias.

Further study into "Political biases of named entities and hashtags on twitter" https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-023-00386-6#Sec2 -> we will go with a different methodology, I believe their methodology is far more complicated than necessary? 

https://mediabiasdetector.seas.upenn.edu/ -> people have made nlp llms to detect political bias, tones, etc in news articles, however tweets are a very different form than news articles so I think it is necessary to have a different product/model for detecting bias, tones, etc in tweets.

As more people get their news from social media, it is important to know whether the news they are receiving is biased, and how biased. 

Currently leaning towards 
1. Fetch data using twitter accounts of known right-wing, left-wing, and centralist news sites and individuals (we will ignore hashtags)
2. Embed and tokenize data using word2vec
3. Use embeded data within different models (ex: transformers?)
4. Possibly different NNs for tone, political lean, connect at the end for some form of ensemble learning?, try cross validations? 
