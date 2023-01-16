# skincare-recommender
Content-based recommendation engine that recommends scraped DERMSTORE skincare products based on product ingredients and descriptions

## Architecture:
1) Skincare product data (Moisturizers, Treatments/Serums, Cleansurs/Exfoliators) scraped from [https://dermstore.com] using **Scrapy**
2) Ingredients standardized with [https://skincarisma.com]'s Ingredient Analyzer Tool using **Selenium Webriver**
3) Product ingredient and description texts vectorized using **BERT embeddings** and **TruncatedSVD/TSNE**
4) Products recommended based on highest **Cosine Similarity**


## To Run:
1) Run ```scrapy crawl <spider> -O file_name.csv``` (for each spider)
2) Update Chromedriver path clean_ingredients.py
3) Run ```python3 clean_ingredients.py```
4) Run ```streamlit run app.py```


## App Demo:

![Alt Text](skincare_demo_AdobeExpress.gif)
