Here are the outputs of all 5 models in two directions:

- Informal -> Formal: [all_model_outputs.0](all_model_outputs.0)
- Formal -> Informal: [all_model_outputs.1](all_model_outputs.1) (Note: "1" refers to formal, and "0" informal.)

There are some abbreviations in the above output files, which are explained here:

| Abbrev.       | meaning                                                      | example                                  |
| ------------- | ------------------------------------------------------------ | ---------------------------------------- |
| src           | source sentence (from [test.uniq.1](test.uniq.1))            | I like Rhythm and Blue music .           |
| ca            | Cross Alignment ([Shen et al., 2017](https://papers.nips.cc/paper/7259-style-transfer-from-non-parallel-text-by-cross-alignment.pdf)) | I like salsa and music and <unk>         |
| multi_decoder | Multi-Decoder ([Fu et al., 2018](http://ruiyan.me/pubs/AAAI2018Fu.pdf)) | I like Fall Out of music funny .         |
| style_emb     | Style-Embedding  ([Fu et al., 2018](http://ruiyan.me/pubs/AAAI2018Fu.pdf)) | I like Teen and big songs .              |
| dar           | Delete-And-Retrieve ([Li et al., 2018](https://www.aclweb.org/anthology/N18-1169/)) | oh yeah , I like Rhythm and Blue music . |
| ours          | IMaT ([Jin et al., 2019](https://www.aclweb.org/anthology/D19-1306.pdf)) | I like Storm and blue music .            |

**IMPORTANT:** Note that there exists duplicates in the original test set ([Rao and Tetreault, 2018](https://www.aclweb.org/anthology/N18-1012.pdf)). For *evaluation fairness* and to *save human evaluation efforts*, we unique each test set. And the number of sentences after uniquing becomes:

|                                                     | # sentences (Original) | # sentences (Unique) |
| --------------------------------------------------- | ---------------------- | -------------------- |
| Informal -> Formal (see [test.uniq.0](test.uniq.0)) | 2748                   | 2741                 |
| Formal -> Informal (see [test.uniq.1](test.uniq.1)) | 2701                   | 2700                 |

