# Awesome - Neural Architecture Search

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ![](https://img.shields.io/badge/Last%20Update-May%2025,%202022-blue.svg)

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

 - **FairNAS: Rethinking Evaluation Fairness of Weight Sharing Neural Architecture Search** `Cited by 167` `ICCV` `2021` `Xiaomi AI Lab` `FairNAS` `Supernet Training` [`PDF`](https://openaccess.thecvf.com/content/ICCV2021/papers/Chu_FairNAS_Rethinking_Evaluation_Fairness_of_Weight_Sharing_Neural_Architecture_Search_ICCV_2021_paper.pdf) [`Official Code (Stars 297)`](https://github.com/xiaomi-automl/FairNAS)  ***TL;DR**: Based on inherent unfairness in the supernet training, the authors propose two levels of constraints: expectation fairness and strict fairness. Particularly, strict fairness ensures equal optimization opportunities for all choice blocks throughout the training, which neither overestimates nor underestimates their capacity.*

 - **Zero-Cost Proxies for Lightweight NAS** `Cited by 51` `ICLR` `2021` `Samsung AI Center, Cambridge` `Zero-Cost NAS` [`PDF`](https://openreview.net/pdf?id=0cmMMy8J5q) [`Official Code (Stars 80)`](https://github.com/SamsungLabs/zero-cost-nas)  ***TL;DR**: In this paper, the authors evaluate conventional reduced-training proxies and quantify how well they preserve ranking between neural network models during search when compared with the rankings produced by final trained accuracy.*

 - **AutoFormer: Searching Transformers for Visual Recognition** `Cited by 32` `ICCV` `2021` `Stony Brook University` `Microsoft Research Asia` `AutoFormer` [`PDF`](https://openaccess.thecvf.com/content/ICCV2021/papers/Chen_AutoFormer_Searching_Transformers_for_Visual_Recognition_ICCV_2021_paper.pdf) [`Official Code (Stars 554)`](https://github.com/microsoft/Cream/tree/main/AutoFormer)  ***TL;DR**: The authors propose a new one-shot architecture search framework, namely AutoFormer, dedicated to vision transformer search. AutoFormer entangles the weights of different blocks in the same layers during supernet training. The performance of these subnets with weights inherited from the supernet is comparable to those retrained from scratch.*

 - **Vision Transformer Architecture Search** `Cited by 10` `arXiv` `2021` `The University of Sydney` `SenseTime Research` `Vision Transformer` `Superformer` [`PDF`](https://arxiv.org/pdf/2106.13700.pdf) [`Official Code (Stars 40)`](https://github.com/xiusu/ViTAS)  ***TL;DR**: This paper present a new cyclic weight-sharing mechanism for token embeddings of the Vision Transformers, which enables each channel could more evenly contribute to all candidate architectures.*

 - **Searching the Search Space of Vision Transformer** `Cited by 0` `NeurIPS` `2021` `Institute of Automation, CAS` `Microsoft Research` `AutoFormerV2` `S3` [`PDF`](https://proceedings.neurips.cc/paper/2021/file/48e95c45c8217961bf6cd7696d80d238-Paper.pdf) [`Official Code (Stars 554)`](https://github.com/microsoft/Cream/tree/main/AutoFormerV2)  ***TL;DR**: The authors propose to use neural architecture search to automate this process, by searching not only the architecture but also the search space. The central idea is to gradually evolve different search dimensions guided by their E-T Error computed using a weight-sharing supernet.*



## <a name="2020 Venues">2020 Venues</a>

 - <ins>**Once-for-All: Train One Network and Specialize it for Efficient Deployment**</ins> `Cited by 508` `ICLR` `2020` `Massachusetts Institute of Technology` `Once-for-All` `OFA` [`PDF`](https://openreview.net/forum?id=HylxE1HKwS) [`Official Code (Stars 1.5k)`](https://github.com/mit-han-lab/once-for-all)  ***TL;DR**: Conventional NAS approaches find a specialized neural network and need to train it from scratch for each case.The authors propose to train a once-for-all (OFA) network that supports diverse architectural settings by decoupling training and search, to reduce the cost, which quickly gets a specialized sub-network by selecting from the OFA network without additional training.*

 - **Designing Network Design Spaces** `Cited by 476` `CVPR` `2020` `FAIR` `RegNet` [`PDF`](https://openaccess.thecvf.com/content_CVPR_2020/papers/Radosavovic_Designing_Network_Design_Spaces_CVPR_2020_paper.pdf)  [`Third-party Code (Stars 162)`](https://github.com/signatrix/regnet) ***TL;DR**: Instead of focusing on designing individual network instances, the authors design network design spaces that parametrize populations of networks. The overall process is analogous to classic manual design of networks, but elevated to the design space level.*

 - **Single Path One-Shot Neural Architecture Search with Uniform Sampling** `Cited by 436` `ECCV` `2020` `MEGVII Technology` `SPOS` `Supernet Training` [`PDF`](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123610528.pdf)  [`Third-party Code (Stars 208)`](https://github.com/ShunLu91/Single-Path-One-Shot-NAS) ***TL;DR**: The authors seek to construct a simplified supernet, where all architectures are single paths so that weight co-adaption problem is alleviated. Training is performed by uniform path sampling. All architectures (and their weights) are trained fully and equally.*

 - **FBNetV2: Differentiable Neural Architecture Search for Spatial and Channel Dimensions** `Cited by 151` `CVPR` `2020` `UC Berkeley` `Facebook Inc.` `FBNetV2` [`PDF`](https://openaccess.thecvf.com/content_CVPR_2020/papers/Wan_FBNetV2_Differentiable_Neural_Architecture_Search_for_Spatial_and_Channel_Dimensions_CVPR_2020_paper.pdf) [`Official Code (Stars 724)`](https://github.com/facebookresearch/mobile-vision)  ***TL;DR**: The authors propose a memory and computationally efficient DNAS variant: DMaskingNAS. This algorithm expands the search space by up to 10^14x over conventional DNAS, supporting searches over spatial and channel dimensions that are otherwise prohibitively expensive: input resolution and number of filters.*

 - **EcoNAS: Finding Proxies for Economical Neural Architecture Search** `Cited by 56` `CVPR` `2020` `The University of Sydney` `SenseTime Computer Vision Research Group` `EcoNAS` [`PDF`](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhou_EcoNAS_Finding_Proxies_for_Economical_Neural_Architecture_Search_CVPR_2020_paper.pdf)   ***TL;DR**: The authors observe that most existing proxies exhibit different behaviors in maintaining the rank consistency among network candidates. In particular, some proxies can be more reliable. Inspired by these observations, the authors present a reliable proxy and further formulate a hierarchical proxy strategy that spends more computations on candidate networks that are potentially more accurate.*

 - **FBNetV3: Joint Architecture-Recipe Search using Neural Acquisition Function** `Cited by 41` `arXiv` `2020` `Facebook Inc.` `UC Berkeley` `UNC Chapel Hill` `FBNetV3` [`PDF`](https://arxiv.org/pdf/2006.02049.pdf)   ***TL;DR**: Previous NAS methods search for architectures under one set of training hyper-parameters (i.e., a training recipe), overlooking superior architecture-recipe combinations. To address this, this paper presents Neural Architecture-Recipe Search (NARS) to search both architectures and their corresponding training recipes, simultaneously.*

 - **Semi-Supervised Neural Architecture Search** `Cited by 27` `NeurIPS` `2020` `University of Science and Technology of China` `Microsoft Research Asia` `Semi-Supervised NAS` [`PDF`](https://proceedings.neurips.cc/paper/2020/file/77305c2f862ad1d353f55bf38e5a5183-Paper.pdf)   ***TL;DR**: Neural architecture search (NAS) relies on a good controller to generate promising architectures. However, training the controller requires both abundant and high-quality pairs of architectures and their accuracy, which is costly. In this paper, the authors propose SemiNAS, a semi-supervised NAS approach that leverages numerous unlabeled architectures (without evaluation and thus nearly no cost).*



## <a name="2019 Venues">2019 Venues</a>

 - <ins>**DARTS: Differentiable Architecture Search**</ins> `Cited by 2.5k` `ICLR` `2019` `Carnegie Mellon University` `Google DeepMind` `DARTS` [`PDF`](https://openreview.net/pdf?id=S1eYHoC5FX) [`Official Code (Stars 3.6k)`](https://github.com/quark0/darts)  ***TL;DR**: This paper addresses the scalability challenge of architecture search by formulating the task in a differentiable manner. Unlike conventional approaches of applying evolution or reinforcement learning over a discrete and non-differentiable search space, the proposed method is based on the continuous relaxation of the architecture representation, allowing efficient search of the architecture using gradient descent.*

 - **Regularized Evolution for Image Classifier Architecture Search** `Cited by 2.0k` `AAAI` `2019` `Google Brain` `Evolution` `AmoebaNet` [`PDF`](https://ojs.aaai.org//index.php/AAAI/article/view/4405) [`Official Code (Stars 23.4k)`](https://github.com/google-research/google-research/tree/master/evolution/regularized_evolution_algorithm)  ***TL;DR**: The authors evolve an image classifier---AmoebaNet-A---that surpasses hand-designs for the first time. To do this, they modify the tournament selection evolutionary algorithm by introducing an age property to favor the younger genotypes.*

 - **MnasNet: Platform-Aware Neural Architecture Search for Mobile** `Cited by 1.8k` `CVPR` `2019` `Google Brain` `Google Inc.` `MNASNet` [`PDF`](https://openaccess.thecvf.com/content_CVPR_2019/papers/Tan_MnasNet_Platform-Aware_Neural_Architecture_Search_for_Mobile_CVPR_2019_paper.pdf) [`Official Code (Stars 4.8k)`](https://github.com/tensorflow/tpu/blob/master/models/official/mnasnet/README.md)  ***TL;DR**: The authors propose an automated mobile neural architecture search (MNAS) approach, which explicitly incorporate model latency into the main objective, where latency is directly measures as real-world inference latency by executing the model on mobile phones.*

 - **ProxylessNAS: Direct Neural Architecture Search on Target Task and Hardware** `Cited by 1.2k` `ICLR` `2019` `Massachusetts Institute of Technology` `ProxylessNAS` [`PDF`](https://openreview.net/pdf?id=HylVB3AqYm) [`Official Code (Stars 1.3k)`](https://github.com/MIT-HAN-LAB/ProxylessNAS)  ***TL;DR**: This paper presents ProxylessNAS that can directly learn the architectures for large-scale target tasks and target hardware platforms. The proposed method address the high memory consumption issue of differentiable NAS and reduce the computational cost (GPU hours and GPU memory) to the same level of regular training while still allowing a large candidate set.*

 - **FBNet: Hardware-Aware Efficient ConvNet Design via Differentiable Neural Architecture Search** `Cited by 811` `CVPR` `2019` `UC Berkeley` `Princeton University` `Facebook Inc.` `FBNet` `Latency Table` [`PDF`](https://openaccess.thecvf.com/content_CVPR_2019/papers/Wu_FBNet_Hardware-Aware_Efficient_ConvNet_Design_via_Differentiable_Neural_Architecture_Search_CVPR_2019_paper.pdf) [`Official Code (Stars 724)`](https://github.com/facebookresearch/mobile-vision)  ***TL;DR**: The authors propose a differentiable neural architecture search (DNAS) framework that uses gradient-based methods to optimize ConvNet architectures, by directly considering latency on target devices.*



## <a name="2018 Venues">2018 Venues</a>

 - <ins>**Efficient Neural Architecture Search via Parameters Sharing**</ins> `Cited by 1.9k` `ICML` `2018` `Google Brain` `Carnegie Mellon University` `ENAS` `Reinforcement Learning` [`PDF`](http://proceedings.mlr.press/v80/pham18a/pham18a.pdf)  [`Third-party Code (Stars 2.6k)`](https://github.com/carpedm20/ENAS-pytorch) ***TL;DR**: The proposed method (ENAS) constructs a large computational graph (suprenet), where each subgraph represents a neural network architecture, hence forcing all architectures to share their parameters. Evaluating candidate architectures with these subgraphs and their corresponding parameters would lead to much lower GPU hours (1000x less expensive than existing methods).*



## <a name="2017 Venues">2017 Venues</a>

 - <ins>**Neural Architecture Search with Reinforcement Learning**</ins> `Cited by 4.0k` `ICLR` `2017` `Google Brain` `Reinforcement Learning` [`PDF`](https://openreview.net/pdf?id=r1Ue8Hcxg)  [`Third-party Code (Stars 395)`](https://github.com/titu1994/neural-architecture-search) ***TL;DR**: This is a pioneering work exploits the paradigms of reinforcement learning (RL) to solve NAS problem. To be specific, the authors use a recurrent network to generate the model descriptions of neural networks and train this RNN with reinforcement learning to maximize the expected accuracy of the generated architectures on a validation set.*

 - **Designing Neural Network Architectures using Reinforcement Learning** `Cited by 1.2k` `ICLR` `2017` `Massachusetts Institute of Technology` `Q-learning` `Reinforcement Learning` [`PDF`](https://openreview.net/pdf?id=S1c2cvqee) [`Official Code (Stars 127)`](https://github.com/bowenbaker/metaqnn)  ***TL;DR**: The authors introduce MetaQNN, a meta-modeling algorithm based on reinforcement learning to automatically generate high-performing CNN architectures for a given learning task. The learning agent is trained to sequentially choose CNN layers using -learning with an e-greedy exploration strategy and experience replay*




# <a name="Survey">Survey</a>

 - **Neural Architecture Search: A Survey** `Cited by 1.5k` `JMLR` `2019` `University of Freiburg` `Survey` [`PDF`](https://jmlr.org/papers/volume20/18-598/18-598.pdf)   ***TL;DR**: The authors provide an overview of existing work in this field of research and categorize them according to three dimensions: search space, search strategy, and performance estimation strategy.*




# <a name="Datasets">Datasets</a>

 - **NAS-Bench-101** [`Download Link`](https://github.com/google-research/nasbench) ***TL;DR**: This dataset contains 423,624 unique neural networks exhaustively generated and evaluated from a fixed graph-based search space. Each network is trained and evaluated multiple times on CIFAR-10 at various training budgets and we present the metrics in a queriable API. The current release contains over 5 million trained and evaluated models.* `How to cite:` **NAS-Bench-101: Towards Reproducible Neural Architecture Search** `Cited by 340` `ICML` `2019` `Google Brain` `NAS-Bench-101` [`PDF`](http://proceedings.mlr.press/v97/ying19a/ying19a.pdf)

# <a name="Codebases">Codebases</a>

 - [**D-X-Y/AutoDL-Projects**](https://github.com/D-X-Y/AutoDL-Projects) `Stars 1.4k` `AutoDL` ***TL;DR**: Automated Deep Learning Projects (AutoDL-Projects) is an open source, lightweight, but useful project for everyone. This project implemented several neural architecture search (NAS) and hyper-parameter optimization (HPO) algorithms.*

# <a name="Misc">Misc</a>

 - [**CVPR 2021 WorkShop - 1st Lightweight NAS Challenge and Moving Beyond**](https://cvpr21-nas.com/) `NAS Challenge` ***TL;DR**: The goals of this workshop are to 1) bring together emerging research in the areas of NAS and etc. to discuss open challenges and opportunities ahead; 2) benchmark lightweight NAS in a systematic and realistic approach. This workshop provides [winner solutions](https://cvpr21-nas.com/competition) of lightweight NAS competitions, and the corresponding [submitted papers](https://cvpr21-nas.com/Paper_Submission).*
