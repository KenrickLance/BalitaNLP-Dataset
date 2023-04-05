# BalitaNLP Dataset

A Filipino language dataset for image-conditional language generation and class-conditional image generation. Composed of 351,755 Filipino news articles gathered from Filipino news outlets.

# Download
* [dataset](https://storage.googleapis.com/public-kenricklancebunag/BalitaNLP/2022/BalitaNLP-Dataset.zip)
* images
    * [part1](https://storage.googleapis.com/public-kenricklancebunag/BalitaNLP/2022/BalitaNLP-images_1.zip)
    * [part2](https://storage.googleapis.com/public-kenricklancebunag/BalitaNLP/2022/BalitaNLP-images_2.zip)
    * [part3](https://storage.googleapis.com/public-kenricklancebunag/BalitaNLP/2022/BalitaNLP-images_2.zip)
    * [part4](https://storage.googleapis.com/public-kenricklancebunag/BalitaNLP/2022/BalitaNLP-images_4.zip)

# Dataset Info

Total # of articles: **351,755**

80-10-10 split for training, validation, and testing.

Each entry in the dataset has 8 fields:
* body - Article text
* title - Article title
* website - Name of the news outlet
* category - News category given by the news outlet
* date - Date published
* author - Article author
* url - URL of the article
* img_url - URL of the article image
* img_path - Filename of the image in the dataset

The articles are formatted in a json format like below
```
{
    'body': ['paragraph1', 'paragraph2', ...],
    'title': 'Philippine Swimming League tutuklas ng bagong talento',
    'website': 'Abante',
    'category': 'Sports,
    'date': 'Jul 8, 2019',
    'author': 'Jose Reyes',
    'url': 'https://www.abante.com.ph/2019/04/04/philippine-swimming-league-tutuklas-ng-bagong-talento/',
    'img_url': 'https://www.abante.com.ph/wp-content/uploads/2019/04/abante-swimming.jpg',
    'img_path': 'a14690aff7cba59b358e8c97b684c58f29537e0716caa21bfd511da8996b078c.jpg',
}
```

Every article has a body, title, website, category, url, img_url, and img_path. 32,174 articles do not have an author.
