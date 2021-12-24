# Clairvoyant Prefetching for Machine Learning I/O

There has been significant interest in deep neural networks recently, both from a theoretical and practical perspective.
Many researchers have proposed new schemes and methods to minimize the training time of the networks, especially on high performance computing clusters.
While we have seen tremendous progress in the training times, data loading is often neglected in these works and is becoming a major bottleneck for training.
We expect this trend to continue, as datasets are becoming larger and specialized hardware for accelerating machine learning is more widely deployed.
In this work, we study the data loading problem from a theoretical perspective and use these insights to design and implement a novel machine learning I/O middleware, HDMLP.
The framework provides an easy-to-use, flexible solution that scales well to many nodes and large datasets, which makes it especially suitable for distributed deep learning on supercomputers.
We confirm in theoretical and practical evaluations that the solution delivers better performance than current state-of-the-art approaches (reducing the median stall time by factors of up to 44) while requiring very few changes to existing codebases and supporting a broad range of environments.

## Software
The described software is available at [OpenCoreCH/hdmlp](https://github.com/OpenCoreCH/hdmlp).

## Publication
We published a paper based on this work at Supercomputing 2021: [Clairvoyant Prefetching for Distributed Machine Learning I/O](https://arxiv.org/abs/2101.08734).
```
@inproceedings{dryden2021clairvoyant,
  title={CLairvoyant Prefetching for Distributed Machine Learning {I/O}},
  author={Nikoli Dryden and Roman B\"{o}hringer and Tal Ben-Nun and Torsten Hoefler},
  booktitle={Proceedings of the International Conference for High Performance Computing, Networking, Storage, and Analysis (SC)},
  year={2021},
  eprint={2101.08734},
  archivePrefix={arXiv},
  primaryClass={cs.DC}
}
```
