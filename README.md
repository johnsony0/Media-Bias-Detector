# Media-Bias-Detector

This detector will be heavily influenced by https://medium.com/@danilo.najkov/detecting-political-bias-in-online-articles-using-nlp-and-classification-models-c1a40ec3989b. However this seems to have used Russian news sites for data, I will be scraping data from sites following https://www.allsides.com/media-bias.

Further study into "Political biases of named entities and hashtags on twitter" https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-023-00386-6#Sec2 -> we will go with a different methodology, I believe their methodology is far more complicated than necessary? 

https://mediabiasdetector.seas.upenn.edu/ -> people have made nlp llms to detect political bias, tones, etc in news articles, however tweets are a very different form than news articles so I think it is necessary to have a different product/model for detecting bias, tones, etc in tweets. -> since then twitter is much harder to scalp so we will instead use facebook

https://www.pewresearch.org/journalism/fact-sheet/social-media-and-news-fact-sheet/ -> most adults use facebook and get their news from it

As more people get their news from social media, it is important to know whether the news they are receiving is biased, and how biased. 

Currently leaning towards 
1. Fetch data using facebook accounts of known right-wing, left-wing, and centralist news sites and individuals (we will ignore hashtags)
2. Embed and tokenize data using word2vec
3. Use embeded data within different models (ex: transformers?)
4. Possibly different NNs for tone, political lean, connect at the end for some form of ensemble learning?, try cross validations?

Tentative Schedule
1. Data (look for available database? likely will have to scrape my own though) 8/25 - 8/28 or 8/29
   - use snscrape
3. Build encoding + Model 8/29 or 8/30 - 9/2 or 9/3
4. Build frontend 9/3 or 9/4 - 9/7

Actual Schedule
1. Data (look for available database? likely will have to scrape my own though) 8/27 - 8/29
2. Build encoding + Model 8/30 - 9/3
3. Break 9/5 - 9/9
4. Enhancing Model 9/10 - 9/10
5. Build frontend 9/11 - 9/12

