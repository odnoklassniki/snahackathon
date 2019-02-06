# [SNA Hackathon 2019](https://snahackathon.org)

Here you can find baselines, kernels and other supplementary materials for SNA Hackathon 2019 event. The event is based on news feed ranking challenge split into three parts:

* Ranking feeds based on features, extracted from photos.
* Ranking feeds based on features, extracted from texts.
* Ranking feeds based on collaborative features.

Details are available available at https://mlbootcamp.ru/round/17/tasks/.

Content of the package:

* Images.ipynb - baseline for images task based on "catability" (we estimate the probability that there is a cat on an image using [YOLOV3 network](https://gluon-cv.mxnet.io/build/examples_detection/demo_yolo.html) and rank items according to catability).
* Texts.ipnynb - baseline for texts combining [gensim Doc2Vec](https://radimrehurek.com/gensim/models/doc2vec.html) with logistic regression for ranking.
* Collaborative.ipynb - simple baseline for collaborative task, ranking with logistic regression on top features.

More readings
* [The short history of a smart news feed](https://habr.com/ru/company/mailru/blog/438392/)