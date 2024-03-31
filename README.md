# Awesome Imbalanced Learning on Graphs
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)]([https://github.com/ZhiningLiu1998/awesome-imbalanced-learning](https://github.com/yanliang3612/awesome-imbalanced-learning-on-graphs)) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

This repository contains a collection of resources and papers on ***Imbalance Learning On Graphs***😆. We are pleased to see that more and more efforts have been devoted to dealing with imbalanced graph-structured data since 2020, which is more complicated than images and text. For a more comprehensive overview of imbalanced learning on various data, please refer to [Awesome-Imbalanced-Learning](https://github.com/ZhiningLiu1998/awesome-imbalanced-learning). 

If you have any relevant paper or codes to update the list, please pull a request or report an issue. 

![image](image/dalle3.png)


# Contents
- [Survery](#survery)
- [Quantity Imbalance](#quantity-imbalance)
  - [Data-Augmentation](#data-augmentation)
  - [Over-Sampling](#over-sampling)
  - [Loss function Engineering](#loss-function-engineering)
  - [Knowledge Distillation Technique](#knowledge-distillation-technique)
  - [Self-Supervised Learning](#self-supervised-learning)
  - [Reinforcement Learning](#reinforcement-learning)
- [Degree Imbalance](#degree-imbalance)
  - [Semi-Supervised Learning](#semi-supervised-learning)
  - [Unsupervised Learning](#unsupervised-learning)
- [Topology Imbalance](#topology-imbalance)
- [Graph Classification](#graph-classification)
- [Multi-modal Learning](#multi-modal-learning)







# Papers
## Quantity Imbalance 
### Data Augmentation
**Rethinking Semi-Supervised Imbalanced Node Classification from Bias-Variance Decomposition**  
> *Divin Yan, Gengchen Wei, Chen Yang, Shengzhong Zhang, Zengfeng Huang* \
> NeurIPS 2023. [[paper](https://arxiv.org/abs/2310.18765)] [[code](https://github.com/yanliang3612/ReVar)]\
> 21 Sep 2023

### Over-Sampling

**INS-GNN: Improving graph imbalance learning with self-supervision**  
> *Xin Juan, Fengfeng Zhou, Wentao Wang, Wei Jin, Jiliang Tang, Xin Wang* \
> Information Sciences. [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0020025523005042)]\
> 30 Aug 2023

**GraphSHA: Synthesizing Harder Samples for Class-Imbalanced Node Classification**  
> *Wen-Zhi Li, Chang-Dong Wang, Hui Xiong, Jian-Huang Lai* \
> KDD 2023. [[paper](https://arxiv.org/abs/2306.09612)]\
> 16 Jun 2023


**GraphSR: A Data Augmentation Algorithm for Imbalanced Node Classification**  
> *Mengting Zhou, Zhiguo Gong* \
> AAAI 2023. [[paper](https://arxiv.org/abs/2302.12814)]\
> 24 Feb 2023

**UNREAL: Unlabled Nodes Retrieval and Labeling for Heavily-imbalanced Node Classification**  
> *Divin Yan, Shengzhong Zhang, Bisheng Li, Min Zhou, Zengfeng Huang* \
> Openreview 2022. [[paper](https://arxiv.org/abs/2303.10371)]\
> 30 Sep 2022

**GraphENS: Neighbor-aware ego network synthesis for class-imbalanced node classification**  
> *Joonhyung Park<sup>1</sup>, Jaeyun Song<sup>1</sup>, Eunho Yang* \
> ICLR 2022. [[paper](https://openreview.net/forum?id=MXEl7i-iru)] [[code](https://github.com/JoonHyung-Park/GraphENS)]\
> 18 Aug 2022

**GraphMixup: Improving Class-Imbalanced Node Classification on Graphs by Self-supervised Context Prediction** 
> *Lirong Wu, Haitao Lin, Zhangyang Gao, Cheng Tan, Stan.Z.Li* \
> ECML-PKDD 2022. [[Paper](https://arxiv.org/abs/2106.11133)] [[code](https://github.com/LirongWu/GraphMixup)] \
> 21 Jun 2021

**ImGAGN:Imbalanced Network Embedding via Generative Adversarial Graph Networks**  
> *Liang Qu, Huaisheng Zhu, Ruiqi Zheng, Yuhui Shi, Hongzhi Yin* \
> KDD 2021. [[paper](https://arxiv.org/abs/2106.02817)] [[code](https://github.com/Leo-Q-316/ImGAGN)]\
> 05 Jun 2021

**GraphSMOTE: Imbalanced Node Classification on Graphs with Graph Neural Networks**      
> *Tianxiang Zhao, Xiang Zhang, Suhang Wang,* \
> WSDM 2021. [[paper](https://arxiv.org/abs/2103.08826)] [[code](https://github.com/TianxiangZhao/GraphSmote)]\
> 16 Mar 2021

**Multi-Class Imbalanced Graph Convolutional Network Learning**   
> *Min Shi, Yufei Tang, Xingquan Zhu, David Wilson, Jianxun Liu* \
> IJCAI 2020. [[paper](https://arxiv.org/abs/2210.05274)] [[code](https://github.com/codeshareabc/DRGCN)] \
> 07 Jan 2021



### Loss Function Engineering

**Hyperbolic Geometric Graph Representation Learning for Hierarchy-imbalance Node Classification**   
> *Xingcheng Fu, Yuecen Wei, Qingyun Sun, Haonan Yuan, Jia Wu, Hao Peng, Jianxin Li* \
> WWW 2023. [[paper](https://arxiv.org/abs/2304.05059)] \
> 11 Apr 2023

**Minority-Weighted Graph Neural Network for Imbalanced Node Classification in Social Networks of Internet of People**   
> *Kefan Wang, Jing An, Mengchu Zhou, Zhe Shi, Xudong Shi, Qi Kang* \
> IEEE Internet of Things Journal. [[paper](https://ieeexplore.ieee.org/abstract/document/9875203)] \
> 01 Jun 2022


**TAM: Topology-Aware Margin Loss for Class-Imbalanced Node Classification**   
> *Jaeyun Song<sup>1</sup>, Joonhyung Park<sup>1</sup>, Eunho Yang* \
> ICML 2022. [[paper](https://arxiv.org/abs/2206.01729)] [[code](https://github.com/Jaeyun-Song/TAM)] \
> 01 Jun 2022


**BA-GNN: On Learning Bias-Aware Graph Neural Network**   
> *Zhengyu Chen, Teng Xiao, Kun Kuang* \
> ICDE 2022. [[paper](https://ieeexplore.ieee.org/document/9835653)]  \
> 09 May 2022


**FRAUDRE: Fraud Detection Dual-Resistant to Graph Inconsistency and Imbalance**   
> *Ge Zhang, Jia Wu, Jian Yang, Amin Beheshti, Shan Xue, Chuan Zhou, Quan Z. Sheng* \
> ICDM 2021. [[paper](https://ieeexplore.ieee.org/document/9679178)] [[github](https://github.com/FraudDetection/FRAUDRE)] \
> 07 Dec 2021




### Knowledge Distillation Technique

**LTE4G: Long-Tail Experts for Graph Neural Networks** 
> *Sukwon Yun, Kibum Kim, Kanghoon Yoon, Chanyoung Park* \
> CIKM 2021. [[paper](https://arxiv.org/abs/2208.10205)] [[github](https://github.com/SukwonYun/LTE4G)] \
> 19 Apr 2022

### Self-Supervised Learning


**Co-Modality Graph Contrastive Learning for Imbalanced Node Classification** 
> *Yiyue Qian, Chunhui Zhang, Yiming Zhang, Qianlong Wen, Yanfang Ye, Chuxu Zhang* \
> NeurIPS 2022. [[paper](https://openreview.net/forum?id=f_kvHrM4Q0)] [[github](https://github.com/graphprojects/CM-GCL)] \
> 01 Nov 2022


**Distance-wise Prototypical Graph Neural Network in Node Imbalance Classification** 
> *Yu Wang, Charu Aggarwal, Tyler Derr* \
> arXiv 2021. [[paper](https://arxiv.org/abs/2110.12035)] [[github](https://github.com/YuWVandy/DPGNN)] \
> 19 Apr 2022

### Reinforcement Learning

**AUC-oriented Graph Neural Network for Fraud Detection** 
> *Mengda Huang , Yang Liu , Xiang Ao , Kuan Li , Jianfeng Chi , Jinghua Feng , Hao Yang , Qing He* \
> WWW 2022. [[paper](https://dl.acm.org/doi/10.1145/3485447.3512178)] \
> 25 Apr 2022



## Degree Imbalance
### Semi-Supervised Learning

**Toward Degree Bias in Embedding-Based Knowledge Graph Completion** 
> *Harry Shomer, Wei Jin, Wentao Wang, Jiliang Tang* \
> WWW 2023. [[paper](https://arxiv.org/abs/2302.05044)]\
> 10 Feb 2023

**ResNorm: Tackling Long-tailed Degree Distribution Issue in Graph Neural Networks via Normalization** 
> *Langzhang Liang, Zenglin Xu, Zixing Song, Irwin King, Jieping Ye* \
> arXiv 2022. [[paper](https://arxiv.org/abs/2206.08181)]\
> 16 Jun 2022

**BA-GNN: On Learning Bias-Aware Graph Neural Network**   
> *Zhengyu Chen, Teng Xiao, Kun Kuang* \
> ICDE 2022. [[paper](https://ieeexplore.ieee.org/document/9835653)]  \
> 09 May 2022

**LTE4G: Long-Tail Experts for Graph Neural Networks** 
> *Sukwon Yun, Kibum Kim, Kanghoon Yoon, Chanyoung Park* \
> CIKM 2021. [[paper](https://arxiv.org/abs/2208.10205)] [[code](https://github.com/SukwonYun/LTE4G)] \
> 19 Apr 2022


**RawlsGCN: Towards Rawlsian Difference Principle on Graph Convolutional Network** 
> *Jian Kang, Yan Zhu, Yinglong Xia, Jiebo Luo, Hanghang Tong* \
> WWW 2022. [[paper](https://arxiv.org/abs/2202.13547)] [[code](https://github.com/jiank2/RawlsGCN)]\
> 28 Feb 2022

**Bilateral Filtering Graph Convolutional Network for Multi-relational Social Recommendation in the Power-law Networks** 
> *Minghao Zhao, Qilin Deng, Kai Wang, Runze Wu, Jianrong Tao, Changjie Fan, Liang Chen, Peng Cui* \
> TOIS 2021. [[paper](https://dl.acm.org/doi/10.1145/3469799)]\
> 21 Sep 2021

**Tail-GNN: Tail-Node Graph Neural Networks** 
> *Zemin Liu, Trung-Kien Nguyen, Yuan Fang* \
> KDD 2021. [[paper](https://dl.acm.org/doi/10.1145/3447548.3467276)] [[code](https://github.com/shuaiOKshuai/Tail-GNN)]\
> 14 Aug 2021


**Towards locality-aware meta-learning of tail node embeddings on networks** 
> *Zemin Liu, Wentao Zhang, Yuan Fang, Xinming Zhang, Steven C.H. Hoi* \
> CIKM 2020. [[paper](https://dl.acm.org/doi/10.1145/3340531.3411910)] [[code](https://github.com/smufang/meta-tail2vec)] \
> 19 Oct 2020

**Investigating and Mitigating Degree-Related Biases in Graph Convolutional Networks** 
> *Xianfeng Tang, Huaxiu Yao, Yiwei Sun, Yiqi Wang, Jiliang Tang, Charu Aggarwal, Prasenjit Mitra, Suhang Wang* \
> CIKM 2020. [[paper](https://arxiv.org/abs/2006.15643)]\
> 28 Jun 2020








### Unsupervised Learning

**Uncovering the Structural Fairness in Graph Contrastive Learning** 
> *Ruijia Wang, Xiao Wang, Chuan Shi, Le Song* \
> NeurIPS 2022. [[paper](https://arxiv.org/abs/2210.03011)] [[code](https://github.com/BUPT-GAMMA/Uncovering-the-Structural-Fairness-in-Graph-Contrastive-Learning)]\
> 06 Oct 2022






## Topology Imbalance
**Topology Uncertainty Modeling For Imbalanced Node Classification on Graphs** 
> *Jiayi Gao, Jiaxing Li, Ke Zhang, Youyong Kong*\
> ICASSP 2023. [[paper](https://ieeexplore.ieee.org/abstract/document/10094813)]\
> 05 May 2023

**Position-aware Structure Learning for Graph Topology-imbalance by Relieving Under-reaching and Over-squashing** 
> *Qingyun Sun, Jianxin Li, Haonan Yuan, Xingcheng Fu, Hao Peng, Cheng Ji, Qian Li, Philip S. Yu*\
> CIKM 2022. [[paper](https://arxiv.org/abs/2208.08302)]\
> 17 Aug 2022

**TopoImb: Toward Topology-level Imbalance in Learning from Graphs** 
> *Tianxiang Zhao, Dongsheng Luo, Xiang Zhang, Suhang Wang*\
> LOG 2022. [[paper](https://openreview.net/forum?id=nR3rZ4ODtQ)]\
> 23 Nov 2022

**Position-aware Structure Learning for Graph Topology-imbalance by Relieving Under-reaching and Over-squashing** 
> *Qingyun Sun, Jianxin Li, Haonan Yuan, Xingcheng Fu, Hao Peng, Cheng Ji, Qian Li, Philip S. Yu* \
> CIKM 2022. [[paper](https://arxiv.org/abs/2208.08302)] [[code](https://github.com/RingBDStack/PASTEL)] \
> 17 Aug 2022


**Topology-Imbalance Learning for Semi-Supervised Node Classification** 
> *Deli Chen, Yankai Lin, Guangxiang Zhao, Xuancheng Ren, Peng Li, Jie Zhou, Xu Sun*\
> NeurIPS 2021. [[paper](https://arxiv.org/abs/2110.04099)] [[code](https://github.com/victorchen96/ReNode)] \
> 08 Oct 2021





## Graph Classification

**Imbalanced Graph Classification via Graph-of-Graph Neural Networks** 
> *Yu Wang, Yuying Zhao, Neil Shah, Tyler Derr* \
> CIKM 2022.  [[paper](https://dl.acm.org/doi/abs/10.1145/3511808.3557356)] [[code](https://github.com/YuWVandy/G2GNN)]\
> 17 Oct 2022


**On Size-Oriented Long-Tailed Graph Classification of Graph Neural Networks** 
> *Zemin Liu, Qiheng Mao, Chenghao Liu, Yuan Fang, Jianling Sun* \
> WWW 2022. [[paper](https://dl.acm.org/doi/10.1145/3485447.3512197)] [[code](https://github.com/shuaiOKshuai/SOLT-GNN)]\
> 25 Apr 2022


## Multi-modal Learning

**Co-Modality Graph Contrastive Learning for Imbalanced Node Classification** 
> *Yiyue Qian, Chunhui Zhang, Yiming Zhang, Qianlong Wen, Yanfang Ye, Chuxu Zhang* \
> NeurIPS 2022.  [[paper](https://openreview.net/forum?id=f_kvHrM4Q0)] [[code](https://github.com/graphprojects/CM-GCL)]\
> 15 Sept 2022


# Contact
- [Divin Yan (yanliangfdu@gmail.com)](https://divinyan.com).
