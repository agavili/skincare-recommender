# skincare-recommender
Content-based recommendation engine that recommends scraped DERMSTORE skincare products based on product ingredients and descriptions


## To Run:
1) Run ```scrapy crawl <spider> -O file_name.csv``` (for each spider)
2) Update Chromedriver path clean_ingredients.py
3) Run ```python3 clean_ingredients.py```
4) Run ```streamlit run app.py```
