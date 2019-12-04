This is the output of all 5 models.

| Abbrev.       | meaning                                                      | example                                  |
| ------------- | ------------------------------------------------------------ | ---------------------------------------- |
| src           | source sentence (from [test.uniq.1](test.uniq.1))            | I like Rhythm and Blue music .           |
| ca            | Cross Alignment ([Shen et al., 2017](https://papers.nips.cc/paper/7259-style-transfer-from-non-parallel-text-by-cross-alignment.pdf)) | I like salsa and music and <unk>         |
| multi_decoder | Multi-Decoder ([Fu et al., 2018](http://ruiyan.me/pubs/AAAI2018Fu.pdf)) | I like Fall Out of music funny .         |
| style_emb     | Style-Embedding  ([Fu et al., 2018](http://ruiyan.me/pubs/AAAI2018Fu.pdf)) | I like Teen and big songs .              |
| dar           | Delete-And-Retrieve ([Li et al., 2018](https://www.aclweb.org/anthology/N18-1169/)) | oh yeah , I like Rhythm and Blue music . |
| ours          | IMaT ([Jin et al., 2019](https://www.aclweb.org/anthology/D19-1306.pdf)) | I like Storm and blue music .            |

Note that there are duplicates in the test set. For evaluation fairness and to save human evaluation efforts, we unique each test set. And the number of sentences after uniquing becomes:

|                                              | # sentences (Original) | # sentences (Unique) |
| -------------------------------------------- | ---------------------- | -------------------- |
| Formal -> Informal: [test.uniq.0](test.uniq.0) | 2748                   | 2741                 |
| Informal -> Formal: [test.uniq.1](test.uniq.1) | 2701                   | 2700                 |

