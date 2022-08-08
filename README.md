# Don't Forget Cheap Training Signals Before Building Unsupervised Bilingual Word Embeddings.

Bilingual Word Embeddings (BWEs) are one of the cornerstones of cross-lingual transfer of NLP models. They can be built using only monolingual corpora without supervision leading to numerous works focusing on unsupervised BWEs. However, most of the current approaches to build unsupervised BWEs do not compare their results with methods based on easy-to-access cross-lingual signals. In this paper, we argue that such signals should always be considered when developing unsupervised BWE methods. The two approaches we find most effective are: 1) using identical words as seed lexicons (which unsupervised approaches incorrectly assume are not available for orthographically distinct language pairs) and 2) combining such lexicons with pairs extracted by matching romanized versions of words with an edit distance threshold. We experiment on thirteen non-Latin languages (and English) and show that such cheap signals work well and that they outperform using more complex unsupervised methods on distant language pairs such as Chinese, Japanese, Kannada, Tamil, and Thai. In addition, they are even competitive with the use of high-quality lexicons in supervised approaches. Our results show that these training signals should not be neglected when building BWEs, even for distant languages.


Repo
--------
* Romanization (Uroman+Levenshtein) dictionaries (minimum normalized edit distance 0.8).
* Identical-pairs dictionaries.


Publication
--------

If you use the code, please cite 

```
@inproceedings{severini2022don,
    title = "Don't Forget Cheap Training Signals Before Building Unsupervised Bilingual Word Embeddings",
    author = {Severini, Silvia and Hangya, Viktor and Sabet, Masoud Jalili and Fraser, Alexander and
      Sch{\"u}tze, Hinrich},
    booktitle={Proceedings of the 15th Workshop on Building and Using Comparable Corpora},
    year = "2022",
}
```

License
-------

Copyright (C) 2022, Silvia Severini

A full copy of the license can be found in LICENSE.
