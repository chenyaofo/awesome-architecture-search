# Awesome - Neural Architecture Search

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ![](https://img.shields.io/badge/Last%20Update-Mar%2012,%202022-blue.svg)

This repo provides an up-to-date list of progress made in Neural architecture search, which includes but not limited to papers, datasets, codebases, frameworks and etc. Please feel free to [open an issue](https://github.com/chenyaofo/awesome-architecture-search/issues) to add new progress.


**Note**: The papers are grouped by published year. In each group, the papers are sorted by their citations. In addition, the paper with <ins>underline</ins> means a milestone in the field. The third-party code prefers `PyTorch`. If you are interested in manually-deisgned architectures, please refer to my another repo [awesome-architecture-search](https://github.com/chenyaofo/awesome-vision-architecture).

 - <a href="#Main Progress">Main Progress</a>
   - <a href="#2017 Venues">2017 Venues</a>
 - <a href="#Survey">Survey</a>
 - <a href="#Datasets">Datasets</a>
 - <a href="#Codebases">Codebases</a>
 - <a href="#Misc">Misc</a>

# <a name="Main Progress">Main Progress</a>

## <a name="2017 Venues">2017 Venues</a>

 - <ins>**Neural Architecture Search with Reinforcement Learning**</ins> `Cited by 3.7k` `ICLR` `2017` `Google Brain` `Reinforcement Learning` [`PDF`](https://openreview.net/pdf?id=r1Ue8Hcxg)  [`Third-party Code (Stars 390)`](https://github.com/titu1994/neural-architecture-search) ***TL;DR**: This is a pioneering work exploits the paradigms of reinforcement learning (RL) to solve NAS problem. To be specific, the authors use a recurrent network to generate the model descriptions of neural networks and train this RNN with reinforcement learning to maximize the expected accuracy of the generated architectures on a validation set.*

 - **Designing Neural Network Architectures using Reinforcement Learning** `Cited by 1.1k` `ICLR` `2017` `Massachusetts Institute of Technology` `Q-learning` `Reinforcement Learning` [`PDF`](https://openreview.net/pdf?id=S1c2cvqee) [`Official Code (Stars 125)`](https://github.com/bowenbaker/metaqnn)  ***TL;DR**: The authors introduce MetaQNN, a meta-modeling algorithm based on reinforcement learning to automatically generate high-performing CNN architectures for a given learning task. The learning agent is trained to sequentially choose CNN layers using -learning with an e-greedy exploration strategy and experience replay*




# <a name="Survey">Survey</a>

 - **Neural Architecture Search: A Survey** `Cited by 1.4k` `JMLR` `2019` `University of Freiburg` `Survey` [`PDF`](https://jmlr.org/papers/volume20/18-598/18-598.pdf)   ***TL;DR**: The authors provide an overview of existing work in this field of research and categorize them according to three dimensions: search space, search strategy, and performance estimation strategy.*




# <a name="Datasets">Datasets</a>

 - **NAS-Bench-101** [`Download Link`](https://github.com/google-research/nasbench) ***TL;DR**: This dataset contains 423,624 unique neural networks exhaustively generated and evaluated from a fixed graph-based search space. Each network is trained and evaluated multiple times on CIFAR-10 at various training budgets and we present the metrics in a queriable API. The current release contains over 5 million trained and evaluated models.* `How to cite:` **NAS-Bench-101: Towards Reproducible Neural Architecture Search** `Cited by 322` `ICML` `2019` `Google Brain` `NAS-Bench-101` [`PDF`](http://proceedings.mlr.press/v97/ying19a/ying19a.pdf)

# <a name="Codebases">Codebases</a>

 - [**D-X-Y/AutoDL-Projects**](https://github.com/D-X-Y/AutoDL-Projects) `Stars 1.3k` `AutoDL` ***TL;DR**: Automated Deep Learning Projects (AutoDL-Projects) is an open source, lightweight, but useful project for everyone. This project implemented several neural architecture search (NAS) and hyper-parameter optimization (HPO) algorithms.*
