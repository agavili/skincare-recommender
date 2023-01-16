# skincare-recommender
Content-based recommendation engine that recommends scraped DERMSTORE skincare products based on product ingredients and descriptions

## Architecture:
1) Skincare product data scraped from dermstore.com using **Scrapy**
2) Standardized ingredients with skincarisma.com's Ingredient Analyzer Tool using **Selenium Webriver**
3) Vectorized product ingredients and descriptions using **BERT embeddings** and **TruncatedSVD/TSNE**
4) Recommended products based on highest **Cosine Similarity**


## To Run:
1) Run ```scrapy crawl <spider> -O file_name.csv``` (for each spider)
2) Update Chromedriver path clean_ingredients.py
3) Run ```python3 clean_ingredients.py```
4) Run ```streamlit run app.py```


## App Demo:

![Alt Text](skincare_demo_AdobeExpress.gif)
