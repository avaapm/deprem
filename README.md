# Tweets Under the Rubble: Detection of Messages Calling for Help in Earthquake Disaster

This repository contains our efforts to detect tweets calling for help, specifically after the 2023 Turkiye-Syria Earthquake. 

## Demonstration (demo_video.zip)
The video demonstration of our tool is given at **demo_video.zip**.

## Dataset (dataset.tsv)
The annotated dataset is given at **dataset.tsv**. We annotate **1,000 tweets in Turkish** if tweets call for help (i.e. request rescue, supply, or donation), and their entity tags (person, city, address, status).
| Column Name  | Description |
| ------------- | ------------- |
| label | Human annotation if tweet calls for help (binary classification) |
| entities | Human annotation of entity tags (i.e. person, city, address, and status). The format is [START_INDEX]:[END_INDEX]%[TAG_TYPE]. |
| tweet_id | Tweet ID from Twitter API. |
| text | Tweet text. |
| quote | If tweet quotes another tweet, we also provide the quoted tweet's text. |

Distibution of tweets in the dataset is as follows:

| Label | Tweet Count | ADDRESS | CITY | PERSON | STATUS |
|----------|----------|----------|----------|----------|----------|
| Call for Help | 418 | 516 | 504 | 364 | 392 |
| Not Call for Help | 582 | - | - | - | - |
| Total | 1,000 tweets | 1,776 tags | - | - | - |

## Keywords
The keyword lists that we use to collect tweets are given in **general_keywords.txt** and **help_keywords.txt**.

## Citation
If you make use of this dataset, please cite following paper.

```bibtex
@InProceedings{toraman2022large,
  author    = {Toraman, Cagri and Kucukkaya, Izzet Emre and Ozcelik, Oguzhan and Sahin, Umitcan},
  title     = {Tweets Under the Rubble: Detection of Messages Calling for Help in Earthquake Disaster},
  year={2023},
  eprint={xxxx.xxxxx},
  archivePrefix={arXiv},
  primaryClass={cs.SI}
}

```
