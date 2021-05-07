# NER-MMTD
Named-entity recognition corpora for french / english voice recognition in the music industry based on the Million Musical Tweets dataset

## Steps

- Clone the project
- Download the MMTD corpora [here](http://www.cp.jku.at/datasets/MMTD/)
- Extract the files `artists.txt` and `track.txt` into `data/raw`
- If you want to generate the corpora again run `python getInfos.py`

## State-of-the-art

Using Flair and CRF on 100 epochs (1.5 hours on a E5-2690 v1):

|                  | precision | recall | f1-core |
|------------------|-----------|--------|---------|
| ARTIST           | 98.10%    | 100%   | 99.06%  |
| PAUSE            | 100%      | 100%   | 100%    |
| START            | 100%      | 100%   | 100%    |
| STOP             | 100%      | 100%   | 100%    |
| TRACK            | 99.42%    | 99.42% | 99.42%  |
| F1-score (macro) |           |        | 99.70%  |

## Sources

- http://www.cp.jku.at/datasets/MMTD/
- http://www.diva-portal.se/smash/get/diva2:1010104/FULLTEXT01.pdf

## Citation

If you want to use this corpora in your research, please cite the following ressources:

```BibTeX
@inproceedings{inproceedings,
  author = {Hauger, David and Kosir, Andrej and Tkalčič, Marko and Schedl, Markus},
  year = {2013},
  month = {11},
  pages = {},
  title = {THE MILLION MUSICAL TWEETS DATASET: WHAT CAN WE LEARN FROM MICROBLOGS}
}

@misc{labrak_yanis_ner_mmtd,
  author       = {Labrak Yanis},
  title        = {Named-entity recognition corpora for multilingual voice recognition in the music industry},
  month        = may,
  year         = 2021,
  version      = {1.0},
  publisher    = {GitHub},
  url          = {https://github.com/qanastek/NER-MMTD}
}
```
