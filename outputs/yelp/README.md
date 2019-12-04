Here are the outputs of all 5 models in two directions:

- Positive -> Negative: [all_model_outputs.0](all_model_outputs.0)
- Negative -> Positive: [all_model_outputs.1](all_model_outputs.1) (Note: "1" refers to formal, and "0" informal.)

There are some abbreviations in the above output files, which are explained here:

| Abbrev.       | meaning                                                      | example                                  |
| ------------- | ------------------------------------------------------------ | ---------------------------------------- |
| src           | source sentence (from the [test set](https://github.com/shentianxiao/language-style-transfer/blob/master/data/yelp/sentiment.test.0))            | she was not happy being there .           |
| ca            | Cross Alignment ([Shen et al., 2017](https://papers.nips.cc/paper/7259-style-transfer-from-non-parallel-text-by-cross-alignment.pdf)) | she was not happy to everyone .         |
| multi_decoder | Multi-Decoder ([Fu et al., 2018](http://ruiyan.me/pubs/AAAI2018Fu.pdf)) | she was not happy of there .         |
| style_emb     | Style-Embedding  ([Fu et al., 2018](http://ruiyan.me/pubs/AAAI2018Fu.pdf)) | she was not sucks cooked go there .              |
| dar           | Delete-And-Retrieve ([Li et al., 2018](https://www.aclweb.org/anthology/N18-1169/)) | being very very nice being there . |
| ours          | IMaT ([Jin et al., 2019](https://www.aclweb.org/anthology/D19-1306.pdf)) | she was very happy with there .            |

