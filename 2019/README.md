# [SNA Hackathon 2019](https://snahackathon.org)

Here you can find baselines, kernels and other supplementary materials for SNA Hackathon 2019 event. The event is based on news feed ranking challenge split into three parts:

* Ranking feeds based on features, extracted from photos.
* Ranking feeds based on features, extracted from texts.
* Ranking feeds based on collaborative features.

Details are available available at https://mlbootcamp.ru/round/17/tasks/.

All baselines here are written using python 3.7 and based on the [Apache Arrow](https://arrow.apache.org) for reading parquet files (see [manual](https://arrow.apache.org/docs/python/install.html) for installation). Image processing is implemented using [MXNet](https://mxnet.incubator.apache.org) framework (see [manual](https://mxnet.incubator.apache.org/versions/master/install/index.html?platform=MacOS&language=Python&processor=CPU) for instllation) and [GluonCV](https://mxnet.incubator.apache.org/versions/master/gluon/index.html). Texts are processed using [Gensim](https://radimrehurek.com/gensim/) package (see [manual](https://radimrehurek.com/gensim/install.html) for installation).

Content of the package:

* Images.ipynb - baseline for images task based on "catability" (we estimate the probability that there is a cat on an image using [YOLOV3 network](https://gluon-cv.mxnet.io/build/examples_detection/demo_yolo.html) and rank items according to catability).
* Texts.ipnynb - baseline for texts combining [gensim Doc2Vec](https://radimrehurek.com/gensim/models/doc2vec.html) with logistic regression for ranking.
* Collaborative.ipynb - simple baseline for collaborative task, ranking with logistic regression on top features.

More readings
* [The short history of a smart news feed](https://habr.com/ru/company/mailru/blog/438392/)