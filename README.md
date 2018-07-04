# DIRSM
Disaster Image Retrieval from Social Media [DIRSM] -- [Multimedia-Satellite-Task 2017](http://www.multimediaeval.org/mediaeval2017/multimediasatellite/)

This code was conceived for the Disaster Image Retrieval from Social Media [DIRSM] subtask, part of the Multimedia-Satellite-Task (MediaEval Benchmark).

It allows fine-tuning of several ConvNets using TensorFlow framework.
Among the networks, it includes:

  - [AlexNet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks)
  - [VGG16](https://arxiv.org/abs/1409.1556)
  - [GoogleNet](https://arxiv.org/abs/1409.4842)
  - [ResNets(50,101,152)](https://arxiv.org/abs/1512.03385) with bootleneck
  - [DenseNets(121,169,201,161)](https://arxiv.org/abs/1608.06993) with bootleneck and compression

DenseNet models were load using [python-torchfile](https://github.com/bshillingford/python-torchfile), ResNets were created using the models available at [tensorflow-resnet](https://github.com/ry/tensorflow-resnet) and, finally, other models were converted to npy with [caffe-tensorflow](https://github.com/ethereon/caffe-tensorflow) and then loaded.

The code also include algorithms for ranking generation and evaluation (Mean Average Precision).

### Citing

If you use this code in your research, please consider citing:

    @inproceedings{multiBrasil_mediaeval,
		author = {Nogueira, Keiller and Fadel, Samuel G. and Dourado, \'{I}caro C. and Werneck, Rafael de O. and Mu\~{n}oz, Javier A. V. and Penatti, Ot\'{a}vio A. B. and Calumby, Rodrigo T. and Li, Lin T. and dos Santos, Jefersson A. and Torres, Ricardo da S.},
		title = {Data-Driven Flood Detection using Neural Networks},
		year = {2017},
		booktitle=medeval,
		location   = {Dublin, Ireland},
		url={http://slim-sig.irisa.fr/me17/Mediaeval_2017_paper_39.pdf},
		pages={2}
	}