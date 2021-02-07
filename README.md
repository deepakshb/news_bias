# News Bias

This project has two components. First, the file scraper.py scrapes more than 1100 articles (not older than 2017) from Times of India news website and stores them in a csv file called news.csv. The second component is a method to find 100 similar words to given word that indicates bias in the articles. After roughly going through the articles, 10 bias words have been selected. In the same component, I performed some text cleaning techniques like punctuation and stopwords removal. Then we create a modal that finds possible phrases from the articles. At last, a Word2Vec skip-gram model is trained with those cleaned articles. Once the training is done, we can evaluate the model and find out the 100 most similar words for each bias word we selected earlier.

Please Note:
1. I have tried to make the output as interactive as possible. The similar words can be seen by selecting options.
2. The Times of India website sometimes responds very slow, therefore sometimes it might take alot of time to scrape all articles. For convienience I have added a dataset generated by the same code scraper.py. But to check the functionality of the program, please delete news.csv file from the project.
