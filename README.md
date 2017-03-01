# SHLO

Shallow baseline models for text implemented in Tensorflow

## Implemented models

* `LinearModel`: Linear model over pretrained embeddings
* `fastText`: [Implementation of fastText in Tensorflow](https://github.com/facebookresearch/fastText)
* `fastTextPreTrained`: fastText initialized with pretrained embeddings
* `TTBB`: [Simple but tough-to-beat-baseline for sentence embeddings](https://openreview.net/pdf?id=SyK00v5xx)
* `TTBBTune`: `TTBB` with tuned embeddings and gradient-tuned common component/smoothing parameter
* `TTBBTuneLazy`: TTBB with tuend embeddings and lazily updated common component (bad)
* `LSTM`: Long short-term memory model
* `SparseLM`: Linear model trained over sparse bag-of-words representation

## Getting started

### Install dependencies

```
pip install --requirement python-package-requirements.txt
```

### Get data

```

chmod +x scripts/get_senna.sh
scripts/get_senna.sh
chmod +x scripts/get_word_freq.sh
scripts/get_word_freq.sh
chmod +x scripts/get_polarity.sh
scripts/get_polarity.sh

```

### Run tests for simple models

```
python shlo_test.py
```

## TODO
[Dan] Add http://nlp.stanford.edu/sentiment/trainDevTestTrees_PTB.zip dataset
