# Awesome - Neural Architecture Search

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ![](https://img.shields.io/badge/Last%20Update-Mar%2021,%202022-blue.svg)

This repo provides an up-to-date list of progress made in Neural architecture search, which includes but not limited to papers, datasets, codebases, frameworks and etc. Please feel free to [open an issue](https://github.com/chenyaofo/awesome-architecture-search/issues) to add new progress.


**Note**: The papers are grouped by published year. In each group, the papers are sorted by their citations. In addition, the paper with <ins>underline</ins> means a milestone in the field. The third-party code prefers `PyTorch`. If you are interested in manually-deisgned architectures, please refer to my another repo [awesome-vision-architecture](https://github.com/chenyaofo/awesome-vision-architecture).

 - <a href="#Main Progress">Main Progress</a>
   - <a href="#2021 Venues">2021 Venues</a>
   - <a href="#2020 Venues">2020 Venues</a>
   - <a href="#2019 Venues">2019 Venues</a>
   - <a href="#2018 Venues">2018 Venues</a>
   - <a href="#2017 Venues">2017 Venues</a>
 - <a href="#Survey">Survey</a>
 - <a href="#Datasets">Datasets</a>
 - <a href="#Codebases">Codebases</a>
 - <a href="#Misc">Misc</a>

# <a name="Main Progress">Main Progress</a>

## <a name="2021 Venues">2021 Venues</a>

 - **FairNAS: Rethinking Evaluation Fairness of Weight Sharing Neural Architecture Search** `Cited by 161` `ICCV` `2021` `Xiaomi AI Lab` `FairNAS` `Supernet Training` [`PDF`](https://openaccess.thecvf.com/content/ICCV2021/papers/Chu_FairNAS_Rethinking_Evaluation_Fairness_of_Weight_Sharing_Neural_Architecture_Search_ICCV_2021_paper.pdf) [`Official Code (Stars 295)`](https://github.com/xiaomi-automl/FairNAS)  ***TL;DR**: Based on inherent unfairness in the supernet training, the authors propose two levels of constraints: expectation fairness and strict fairness. Particularly, strict fairness ensures equal optimization opportunities for all choice blocks throughout the training, which neither overestimates nor underestimates their capacity.*

 - **Zero-Cost Proxies for Lightweight NAS** `Cited by 43` `ICLR` `2021` `Samsung AI Center, Cambridge` `Zero-Cost NAS` [`PDF`](https://openreview.net/pdf?id=0cmMMy8J5q) [`Official Code (Stars 70)`](https://github.com/SamsungLabs/zero-cost-nas)  ***TL;DR**: In this paper, the authors evaluate conventional reduced-training proxies and quantify how well they preserve ranking between neural network models during search when compared with the rankings produced by final trained accuracy.*



## <a name="2020 Venues">2020 Venues</a>

 - <ins>**Once-for-All: Train One Network and Specialize it for Efficient Deployment**</ins> `Cited by 460` `ICLR` `2020` `Massachusetts Institute of Technology` `Once-for-All` `OFA` [`PDF`](https://openreview.net/forum?id=HylxE1HKwS) [`Official Code (Stars 1.5k)`](https://github.com/mit-han-lab/once-for-all)  ***TL;DR**: Conventional NAS approaches find a specialized neural network and need to train it from scratch for each case.The authors propose to train a once-for-all (OFA) network that supports diverse architectural settings by decoupling training and search, to reduce the cost, which quickly gets a specialized sub-network by selecting from the OFA network without additional training.*

 - **Single Path One-Shot Neural Architecture Search with Uniform Sampling** `Cited by 406` `ECCV` `2020` `MEGVII Technology` `SPOS` `Supernet Training` [`PDF`](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123610528.pdf)  [`Third-party Code (Stars 206)`](https://github.com/ShunLu91/Single-Path-One-Shot-NAS) ***TL;DR**: The authors seek to construct a simplified supernet, where all architectures are single paths so that weight co-adaption problem is alleviated. Training is performed by uniform path sampling. All architectures (and their weights) are trained fully and equally.*



## <a name="2019 Venues">2019 Venues</a>

 - <ins>**DARTS: Differentiable Architecture Search**</ins> `Cited by 2.4k` `ICLR` `2019` `Carnegie Mellon University` `Google DeepMind` `DARTS` [`PDF`](https://openreview.net/pdf?id=S1eYHoC5FX) [`Official Code (Stars 3.5k)`](https://github.com/quark0/darts)  ***TL;DR**: This paper addresses the scalability challenge of architecture search by formulating the task in a differentiable manner. Unlike conventional approaches of applying evolution or reinforcement learning over a discrete and non-differentiable search space, the proposed method is based on the continuous relaxation of the architecture representation, allowing efficient search of the architecture using gradient descent.*

 - **Regularized Evolution for Image Classifier Architecture Search** `Cited by 1.9k` `AAAI` `2019` `Google Brain` `Evolution` `AmoebaNet` [`PDF`](https://ojs.aaai.org//index.php/AAAI/article/view/4405) [`Official Code (Stars 22.4k)`](https://github.com/google-research/google-research/tree/master/evolution/regularized_evolution_algorithm)  ***TL;DR**: The authors evolve an image classifier---AmoebaNet-A---that surpasses hand-designs for the first time. To do this, they modify the tournament selection evolutionary algorithm by introducing an age property to favor the younger genotypes.*

 - **ProxylessNAS: Direct Neural Architecture Search on Target Task and Hardware** `Cited by 1.1k` `ICLR` `2019` `Massachusetts Institute of Technology` `ProxylessNAS` [`PDF`](https://openreview.net/pdf?id=HylVB3AqYm) [`Official Code (Stars 1.3k)`](https://github.com/MIT-HAN-LAB/ProxylessNAS)  ***TL;DR**: This paper presents ProxylessNAS that can directly learn the architectures for large-scale target tasks and target hardware platforms. The proposed method address the high memory consumption issue of differentiable NAS and reduce the computational cost (GPU hours and GPU memory) to the same level of regular training while still allowing a large candidate set.*



## <a name="2018 Venues">2018 Venues</a>

 - <ins>**Efficient Neural Architecture Search via Parameters Sharing**</ins> `Cited by 1.8k` `ICML` `2018` `Google Brain` `Carnegie Mellon University` `ENAS` `Reinforcement Learning` [`PDF`](http://proceedings.mlr.press/v80/pham18a/pham18a.pdf)  [`Third-party Code (Stars 2.5k)`](https://github.com/carpedm20/ENAS-pytorch) ***TL;DR**: The proposed method (ENAS) constructs a large computational graph (suprenet), where each subgraph represents a neural network architecture, hence forcing all architectures to share their parameters. Evaluating candidate architectures with these subgraphs and their corresponding parameters would lead to much lower GPU hours (1000x less expensive than existing methods).*



## <a name="2017 Venues">2017 Venues</a>

 - <ins>**Neural Architecture Search with Reinforcement Learning**</ins> `Cited by 3.8k` `ICLR` `2017` `Google Brain` `Reinforcement Learning` [`PDF`](https://openreview.net/pdf?id=r1Ue8Hcxg)  [`Third-party Code (Stars 391)`](https://github.com/titu1994/neural-architecture-search) ***TL;DR**: This is a pioneering work exploits the paradigms of reinforcement learning (RL) to solve NAS problem. To be specific, the authors use a recurrent network to generate the model descriptions of neural networks and train this RNN with reinforcement learning to maximize the expected accuracy of the generated architectures on a validation set.*

 - **Designing Neural Network Architectures using Reinforcement Learning** `Cited by 1.1k` `ICLR` `2017` `Massachusetts Institute of Technology` `Q-learning` `Reinforcement Learning` [`PDF`](https://openreview.net/pdf?id=S1c2cvqee) [`Official Code (Stars 125)`](https://github.com/bowenbaker/metaqnn)  ***TL;DR**: The authors introduce MetaQNN, a meta-modeling algorithm based on reinforcement learning to automatically generate high-performing CNN architectures for a given learning task. The learning agent is trained to sequentially choose CNN layers using -learning with an e-greedy exploration strategy and experience replay*




# <a name="Survey">Survey</a>

 - **Neural Architecture Search: A Survey** `Cited by 1.4k` `JMLR` `2019` `University of Freiburg` `Survey` [`PDF`](https://jmlr.org/papers/volume20/18-598/18-598.pdf)   ***TL;DR**: The authors provide an overview of existing work in this field of research and categorize them according to three dimensions: search space, search strategy, and performance estimation strategy.*




# <a name="Datasets">Datasets</a>

 - **NAS-Bench-101** [`Download Link`](https://github.com/google-research/nasbench) ***TL;DR**: This dataset contains 423,624 unique neural networks exhaustively generated and evaluated from a fixed graph-based search space. Each network is trained and evaluated multiple times on CIFAR-10 at various training budgets and we present the metrics in a queriable API. The current release contains over 5 million trained and evaluated models.* `How to cite:` **NAS-Bench-101: Towards Reproducible Neural Architecture Search** `Cited by 325` `ICML` `2019` `Google Brain` `NAS-Bench-101` [`PDF`](http://proceedings.mlr.press/v97/ying19a/ying19a.pdf)

# <a name="Codebases">Codebases</a>

 - [**D-X-Y/AutoDL-Projects**](https://github.com/D-X-Y/AutoDL-Projects) `Stars 1.3k` `AutoDL` ***TL;DR**: Automated Deep Learning Projects (AutoDL-Projects) is an open source, lightweight, but useful project for everyone. This project implemented several neural architecture search (NAS) and hyper-parameter optimization (HPO) algorithms.*

# <a name="Misc">Misc</a>

 - [**CVPR 2021 WorkShop - 1st Lightweight NAS Challenge and Moving Beyond**](https://cvpr21-nas.com/) `NAS Challenge` ***TL;DR**: The goals of this workshop are to 1) bring together emerging research in the areas of NAS and etc. to discuss open challenges and opportunities ahead; 2) benchmark lightweight NAS in a systematic and realistic approach. This workshop provides [winner solutions](https://cvpr21-nas.com/competition) of lightweight NAS competitions, and the corresponding [submitted papers](https://cvpr21-nas.com/Paper_Submission).*
