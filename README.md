# Awesome Imbalanced Learning on Graphs

<p align="center">
  <a href="https://github.com/yanliang3612/awesome-imbalanced-learning-on-graphs">
    <img src="https://awesome.re/badge.svg" alt="Awesome">
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License: MIT">
  </a>
  <a href="#citation">
    <img src="https://img.shields.io/badge/Cite-BibTeX-blue.svg" alt="Cite with BibTeX">
  </a>
</p>

<p align="center">
  <img src="image/imbalanced-graphs-logo.png" alt="Imbalanced Learning on Graphs logo" width="760">
</p>

<p align="center">
  <strong>A curated collection of surveys, papers, and code for imbalanced learning on graphs.</strong><br>
  <em>Found this list useful? Give it a ⭐ — unlike class labels, GitHub stars are welcome to be wildly imbalanced.</em>
</p>

<p align="center">
  <a href="#surveys">Surveys</a>
  |
  <a href="#node-level-imbalance">Node-level</a>
  |
  <a href="#edge-level-imbalance">Edge-level</a>
  |
  <a href="#graph-level-imbalance">Graph-level</a>
  |
  <a href="#federated-graph-learning">Federated</a>
  |
  <a href="#multimodal-learning">Multimodal</a>
  |
  <a href="#citation">Citation</a>
</p>

Last updated: 2026-07-16

---

## Table of Contents

- [Overview](#overview)
- [Surveys](#surveys)
- [Node-level imbalance](#node-level-imbalance)
  - [Quantity imbalance](#quantity-imbalance)
    - [Data augmentation](#data-augmentation)
    - [Oversampling](#oversampling)
    - [Loss function engineering](#loss-function-engineering)
    - [Knowledge distillation](#knowledge-distillation)
    - [Self-supervised learning](#self-supervised-learning)
    - [Reinforcement learning](#reinforcement-learning)
  - [Community bias](#community-bias)
  - [Degree imbalance](#degree-imbalance)
  - [Topology imbalance](#topology-imbalance)
- [Edge-level imbalance](#edge-level-imbalance)
- [Graph-level imbalance](#graph-level-imbalance)
  - [Graph classification](#graph-classification)
  - [Graph size imbalance](#graph-size-imbalance)
- [Federated graph learning](#federated-graph-learning)
- [Multimodal learning](#multimodal-learning)
- [Citation](#citation)
- [Contributing](#contributing)
- [Contact](#contact)

## Overview

Imbalanced graph learning studies how to learn effectively when graph data is
skewed across classes, node degrees, topology, communities, graph sizes, or
distributed clients. This list organizes representative work by imbalance type
and learning strategy.

**Legend:** Paper titles link to the publication or primary preprint. `Preprint`
links are included when a separate published version exists. `Code` points to
the implementation, and the badge shows its current GitHub star count.

## Surveys

| Title | Venue | Date | Code |
| - | - | - | - |
| [**A Survey of Graph Neural Networks in Real World: Imbalance, Noise, Privacy and OOD Challenges**](https://doi.org/10.1109/TPAMI.2025.3630673)<br>[Preprint](https://arxiv.org/abs/2403.04468) | IEEE TPAMI 2025 | 2025 | - |
| [**A Survey of Imbalanced Learning on Graphs: Problems, Techniques, and Future Directions**](https://doi.org/10.1109/TKDE.2025.3549299)<br>[Preprint](https://arxiv.org/abs/2308.13821) | IEEE TKDE 2025 | 2025 | - |
| [**Class-Imbalanced Learning on Graphs: A Survey**](https://doi.org/10.1145/3718734)<br>[Preprint](https://arxiv.org/abs/2304.04300) | ACM Computing Surveys 2025 | 2025 | - |
| ![Star](https://img.shields.io/github/stars/RingBDStack/IGL-Bench.svg?style=social&label=Star)<br>[**IGL-Bench: Establishing the Comprehensive Benchmark for Imbalanced Graph Learning**](https://proceedings.iclr.cc/paper_files/paper/2025/hash/05b69cc4c8ff6e24c5de1ecd27223d37-Abstract-Conference.html) | ICLR 2025 | 2025 | [GitHub](https://github.com/RingBDStack/IGL-Bench) |

## Node-level imbalance

### Quantity imbalance

#### Data augmentation

| Title | Venue | Date | Code |
| - | - | - | - |
| [**GraphST: Class-Imbalanced Node Classification with Semantic Relation Transfer**](https://doi.org/10.1016/j.patcog.2025.112626) | Pattern Recognition 2026 | 2026.04 | - |
| [**GIER: Addressing Class Imbalance in GNNs Through Experience Replay**](https://doi.org/10.1609/aaai.v40i19.38646) | AAAI 2026 | 2026.03.14 | - |
| [**GraphSB: Boosting Imbalanced Node Classification on Graphs through Structural Balance**](https://arxiv.org/abs/2601.19352) | arXiv 2026 | 2026.01.27 | - |
| [**Graph Neural Network with Generative Adversarial Training for Node Classification on Class Imbalanced Data**](https://doi.org/10.1016/j.engappai.2025.112264) | Engineering Applications of Artificial Intelligence 2025 | 2025.12.12 | - |
| [**GraphIAM: Two-Stage Algorithm for Improving Class-Imbalanced Node Classification on Attribute-Missing Graphs**](https://doi.org/10.1145/3746252.3761086) | CIKM 2025 | 2025.11.10 | - |
| [**GraphIFE: Rethinking Graph Imbalance Node Classification via Invariant Learning**](https://arxiv.org/abs/2509.23616) | arXiv 2025 | 2025.09.28 | - |
| [**When Noisy Labels Meet Class Imbalance on Graphs: A Graph Augmentation Method with LLM and Pseudo Label**](https://arxiv.org/abs/2507.18153) | arXiv 2025 | 2025.07.24 | - |
| ![Star](https://img.shields.io/github/stars/maxin88scu/ImGDA.svg?style=social&label=Star)<br>[**Dual Prototype-Enhanced Contrastive Framework for Class-Imbalanced Graph Domain Adaptation**](https://proceedings.neurips.cc/paper_files/paper/2025/hash/455b24e256981fb97f7a650993c35c98-Abstract-Conference.html) | NeurIPS 2025 | 2025 | [GitHub](https://github.com/maxin88scu/ImGDA) |
| [**Graffin: Stand for Tails in Imbalanced Node Classification**](https://arxiv.org/abs/2409.05339) | arXiv 2024 | 2024.09.09 | - |
| [**HyperSMOTE: A Hypergraph-based Oversampling Approach for Imbalanced Node Classifications**](https://arxiv.org/abs/2409.05402) | arXiv 2024 | 2024.09.09 | - |
| ![Star](https://img.shields.io/github/stars/ZhiningLiu1998/BAT.svg?style=social&label=Star)<br>[**Class-Imbalanced Graph Learning without Class Rebalancing**](https://openreview.net/forum?id=pPnkpvBeZN) | ICML 2024 | 2024.05.02 | [GitHub](https://github.com/ZhiningLiu1998/BAT) |
| [**BuffGraph: Enhancing Class-Imbalanced Node Classification via Buffer Nodes**](https://arxiv.org/abs/2402.13114) | arXiv 2024 | 2024.02.20 | - |
| ![Star](https://img.shields.io/github/stars/yanliang3612/ReVar.svg?style=social&label=Star)<br>[**Rethinking Semi-Supervised Imbalanced Node Classification from Bias-Variance Decomposition**](https://arxiv.org/abs/2310.18765) | NeurIPS 2023 | 2023.09.21 | [GitHub](https://github.com/yanliang3612/ReVar) |
| [**Imbalanced Node Classification Beyond Homophilic Assumption**](https://arxiv.org/abs/2304.14635) | arXiv 2023 | 2023.04.28 | - |

#### Oversampling

| Title | Venue | Date | Code |
| - | - | - | - |
| ![Star](https://img.shields.io/github/stars/ZZY-GraphMiningLab/GraphUAT.svg?style=social&label=Star)<br>[**GraphUAT: An Uncertainty-Driven Pseudo-Labeling Method for Class-Imbalanced Node Classification**](https://doi.org/10.1016/j.eswa.2026.133450) | Expert Systems with Applications 2026 | 2026 | [GitHub](https://github.com/ZZY-GraphMiningLab/GraphUAT) |
| [**Multi-Motif Enhanced Node Representation Generation for Class-Imbalanced Node Classification**](https://doi.org/10.1016/j.neucom.2026.133903) | Neurocomputing 2026 | 2026.05.13 | - |
| [**IMMix: Class-Imbalanced Node Classification via Prototypical Selective Mixup Augmentation**](https://doi.org/10.1016/j.patcog.2025.112749) | Pattern Recognition 2026 | 2026.04 | - |
| ![Star](https://img.shields.io/github/stars/flzeng1/PNS.svg?style=social&label=Star)<br>[**Pure Node Selection for Imbalanced Graph Node Classification**](https://doi.org/10.1016/j.neunet.2025.108315)<br>[Preprint](https://arxiv.org/abs/2509.23662) | Neural Networks 2026 | 2026.04 | [GitHub](https://github.com/flzeng1/PNS) |
| [**A Multi-View Graph Neural Network with Subgraph Variational Autoencoder for Class-Imbalanced Node Classification**](https://doi.org/10.1016/j.knosys.2025.115081) | Knowledge-Based Systems 2026 | 2026.02.15 | - |
| ![Star](https://img.shields.io/github/stars/ZZY-GraphMiningLab/GraphBSSN.svg?style=social&label=Star)<br>[**GraphBSSN: A Simple yet Effective Generative Method for Node Classification in Class-Imbalanced Graphs**](https://doi.org/10.1016/j.knosys.2025.114175) | Knowledge-Based Systems 2025 | 2025 | [GitHub](https://github.com/ZZY-GraphMiningLab/GraphBSSN) |
| ![Star](https://img.shields.io/github/stars/ZhixunLEE/IceBerg.svg?style=social&label=Star)<br>[**Iceberg: Debiased self-training for class-imbalanced node classification**](https://arxiv.org/abs/2502.06280) | WWW 2025 | 2025.02.10 | [GitHub](https://github.com/ZhixunLEE/IceBerg) |
| [**UPL: Uncertainty-aware Pseudo-labeling for Imbalance Transductive Node Classification**](https://arxiv.org/abs/2502.00716) | arXiv 2025 | 2025.02.02 | - |
| [**Overcoming Class Imbalance: Unified GNN Learning with Structural and Semantic Connectivity Representations**](https://arxiv.org/abs/2412.20656) | arXiv 2024 | 2024.12.30 | - |
| [**VIGraph: Generative Self-Supervised Learning for Class-Imbalanced Node Classification**](https://arxiv.org/abs/2311.01191) | arXiv 2023 | 2023.11.02 | - |
| [**INS-GNN: Improving graph imbalance learning with self-supervision**](https://www.sciencedirect.com/science/article/abs/pii/S0020025523005042) | Information Sciences | 2023.08.30 | - |
| [**GraphSHA: Synthesizing Harder Samples for Class-Imbalanced Node Classification**](https://arxiv.org/abs/2306.09612) | KDD 2023 | 2023.06.16 | - |
| [**Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information Networks**](https://dl.acm.org/doi/10.1145/3583780.3615055) | CIKM 2023 | 2023.02.27 | - |
| [**GraphSR: A Data Augmentation Algorithm for Imbalanced Node Classification**](https://arxiv.org/abs/2302.12814) | AAAI 2023 | 2023.02.24 | - |
| [**UNREAL: Unlabled Nodes Retrieval and Labeling for Heavily-imbalanced Node Classification**](https://arxiv.org/abs/2303.10371) | Openreview 2022 | 2022.09.30 | - |
| ![Star](https://img.shields.io/github/stars/JoonHyung-Park/GraphENS.svg?style=social&label=Star)<br>[**GraphENS: Neighbor-aware ego network synthesis for class-imbalanced node classification**](https://openreview.net/forum?id=MXEl7i-iru) | ICLR 2022 | 2022.08.18 | [GitHub](https://github.com/JoonHyung-Park/GraphENS) |
| [**A Graph Neural Network-Based Node Classification Model on Class-Imbalanced Graph Data**](https://doi.org/10.1016/j.knosys.2022.108538) | Knowledge-Based Systems 2022 | 2022.05.23 | - |
| [**Graph Neural Network with Curriculum Learning for Imbalanced Node Classification**](https://arxiv.org/abs/2202.02529) | arXiv 2022 | 2022.02.05 | - |
| ![Star](https://img.shields.io/github/stars/LirongWu/GraphMixup.svg?style=social&label=Star)<br>[**GraphMixup: Improving Class-Imbalanced Node Classification on Graphs by Self-supervised Context Prediction**](https://arxiv.org/abs/2106.11133) | ECML-PKDD 2022 | 2021.06.21 | [GitHub](https://github.com/LirongWu/GraphMixup) |
| ![Star](https://img.shields.io/github/stars/Leo-Q-316/ImGAGN.svg?style=social&label=Star)<br>[**ImGAGN:Imbalanced Network Embedding via Generative Adversarial Graph Networks**](https://arxiv.org/abs/2106.02817) | KDD 2021 | 2021.06.05 | [GitHub](https://github.com/Leo-Q-316/ImGAGN) |
| ![Star](https://img.shields.io/github/stars/TianxiangZhao/GraphSmote.svg?style=social&label=Star)<br>[**GraphSMOTE: Imbalanced Node Classification on Graphs with Graph Neural Networks**](https://arxiv.org/abs/2103.08826) | WSDM 2021 | 2021.03.16 | [GitHub](https://github.com/TianxiangZhao/GraphSmote) |
| ![Star](https://img.shields.io/github/stars/codeshareabc/DRGCN.svg?style=social&label=Star)<br>[**Multi-Class Imbalanced Graph Convolutional Network Learning**](https://arxiv.org/abs/2210.05274) | IJCAI 2020 | 2021.01.07 | [GitHub](https://github.com/codeshareabc/DRGCN) |

#### Loss function engineering

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Enhancing Imbalanced Node Classification via Curriculum-Guided Feature Learning and Three-Stage Attention Network**](https://arxiv.org/abs/2602.03808) | arXiv 2026 | 2026.02.03 | - |
| ![Star](https://img.shields.io/github/stars/afofanah/PIMPC-GNN.svg?style=social&label=Star)<br>[**PIMPC-GNN: Physics-Informed Multi-Phase Consensus Learning for Enhancing Imbalanced Node Classification in Graph Neural Networks**](https://arxiv.org/abs/2602.01920) | arXiv 2026 | 2026.02.02 | [GitHub](https://github.com/afofanah/PIMPC-GNN) |
| ![Star](https://img.shields.io/github/stars/NanChanNN/NodeImport.svg?style=social&label=Star)<br>[**NodeImport: Imbalanced Node Classification with Node Importance Assessment**](https://dl.acm.org/doi/10.1145/3690624.3709215) | KDD 2025 | 2025.07.20 | [GitHub](https://github.com/NanChanNN/NodeImport) |
| [**Meta-GCN: A Dynamically Weighted Loss Minimization Method for Dealing with the Data Imbalance in Graph Neural Networks**](https://arxiv.org/abs/2406.17073) | arXiv 2024 | 2024.06.24 | - |
| ![Star](https://img.shields.io/github/stars/MarcoMarkwald/REFUEL.svg?style=social&label=Star)<br>[**REFUEL: Rule Extraction for Imbalanced Neural Node Classification**](https://doi.org/10.1007/s10994-024-06569-0) | Machine Learning 2024 | 2024.06.19 | [GitHub](https://github.com/MarcoMarkwald/REFUEL) |
| [**Automated Loss Function Search for Class-Imbalanced Node Classification**](https://openreview.net/forum?id=O1hmwi51pp) | ICML 2024 | 2024.05.02 | - |
| [**Hyperbolic Geometric Graph Representation Learning for Hierarchy-imbalance Node Classification**](https://arxiv.org/abs/2304.05059) | WWW 2023 | 2023.04.11 | - |
| [**Minority-Weighted Graph Neural Network for Imbalanced Node Classification in Social Networks of Internet of People**](https://ieeexplore.ieee.org/abstract/document/9875203) | IEEE Internet of Things Journal | 2022.06.01 | - |
| ![Star](https://img.shields.io/github/stars/Jaeyun-Song/TAM.svg?style=social&label=Star)<br>[**TAM: Topology-Aware Margin Loss for Class-Imbalanced Node Classification**](https://arxiv.org/abs/2206.01729) | ICML 2022 | 2022.06.01 | [GitHub](https://github.com/Jaeyun-Song/TAM) |
| [**BA-GNN: On Learning Bias-Aware Graph Neural Network**](https://ieeexplore.ieee.org/document/9835653) | ICDE 2022 | 2022.05.09 | - |
| ![Star](https://img.shields.io/github/stars/FraudDetection/FRAUDRE.svg?style=social&label=Star)<br>[**FRAUDRE: Fraud Detection Dual-Resistant to Graph Inconsistency and Imbalance**](https://ieeexplore.ieee.org/document/9679178) | ICDM 2021 | 2021.12.07 | [GitHub](https://github.com/FraudDetection/FRAUDRE) |
| [**Boosting-GNN: Boosting Algorithm for Graph Networks on Imbalanced Node Classification**](https://doi.org/10.3389/fnbot.2021.775688) | Frontiers in Neurorobotics 2021 | 2021.11.25 | - |

#### Knowledge distillation

| Title | Venue | Date | Code |
| - | - | - | - |
| ![Star](https://img.shields.io/github/stars/SukwonYun/LTE4G.svg?style=social&label=Star)<br>[**LTE4G: Long-Tail Experts for Graph Neural Networks**](https://arxiv.org/abs/2208.10205) | CIKM 2021 | 2022.04.19 | [GitHub](https://github.com/SukwonYun/LTE4G) |

#### Self-supervised learning

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Node Transfer with Graph Contrastive Learning for Class-Imbalanced Node Classification**](https://doi.org/10.1016/j.neunet.2025.107674) | Neural Networks 2025 | 2025.10 | - |
| [**When Sparsity Meets Contrastive Models: Less Graph Data Can Bring Better Class-Balanced Representations**](https://proceedings.mlr.press/v202/zhang23o.html) | ICML 2023 | 2023.07.23 | - |
| ![Star](https://img.shields.io/github/stars/graphprojects/CM-GCL.svg?style=social&label=Star)<br>[**Co-Modality Graph Contrastive Learning for Imbalanced Node Classification**](https://openreview.net/forum?id=f_kvHrM4Q0) | NeurIPS 2022 | 2022.11.01 | [GitHub](https://github.com/graphprojects/CM-GCL) |
| [**ImGCL: Revisiting Graph Contrastive Learning on Imbalanced Node Classification**](https://arxiv.org/abs/2205.11332) | arXiv 2022 | 2022.05.23 | - |
| ![Star](https://img.shields.io/github/stars/YuWVandy/DPGNN.svg?style=social&label=Star)<br>[**Distance-wise Prototypical Graph Neural Network in Node Imbalance Classification**](https://arxiv.org/abs/2110.12035) | arXiv 2021 | 2022.04.19 | [GitHub](https://github.com/YuWVandy/DPGNN) |

#### Reinforcement learning

| Title | Venue | Date | Code |
| - | - | - | - |
| [**AUC-oriented Graph Neural Network for Fraud Detection**](https://dl.acm.org/doi/10.1145/3485447.3512178) | WWW 2022 | 2022.04.25 | - |

### Community bias

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Understanding Community Bias Amplification in Graph Representation Learning**](https://arxiv.org/abs/2312.04883) | arXiv 2023 | 2023.12.08 | - |

### Degree imbalance

#### Semi-supervised learning

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Toward Degree Bias in Embedding-Based Knowledge Graph Completion**](https://arxiv.org/abs/2302.05044) | WWW 2023 | 2023.02.10 | - |
| [**ResNorm: Tackling Long-tailed Degree Distribution Issue in Graph Neural Networks via Normalization**](https://arxiv.org/abs/2206.08181) | arXiv 2022 | 2022.06.16 | - |
| [**BA-GNN: On Learning Bias-Aware Graph Neural Network**](https://ieeexplore.ieee.org/document/9835653) | ICDE 2022 | 2022.05.09 | - |
| ![Star](https://img.shields.io/github/stars/SukwonYun/LTE4G.svg?style=social&label=Star)<br>[**LTE4G: Long-Tail Experts for Graph Neural Networks**](https://arxiv.org/abs/2208.10205) | CIKM 2021 | 2022.04.19 | [GitHub](https://github.com/SukwonYun/LTE4G) |
| ![Star](https://img.shields.io/github/stars/jiank2/RawlsGCN.svg?style=social&label=Star)<br>[**RawlsGCN: Towards Rawlsian Difference Principle on Graph Convolutional Network**](https://arxiv.org/abs/2202.13547) | WWW 2022 | 2022.02.28 | [GitHub](https://github.com/jiank2/RawlsGCN) |
| [**Bilateral Filtering Graph Convolutional Network for Multi-relational Social Recommendation in the Power-law Networks**](https://dl.acm.org/doi/10.1145/3469799) | TOIS 2021 | 2021.09.21 | - |
| ![Star](https://img.shields.io/github/stars/shuaiOKshuai/Tail-GNN.svg?style=social&label=Star)<br>[**Tail-GNN: Tail-Node Graph Neural Networks**](https://dl.acm.org/doi/10.1145/3447548.3467276) | KDD 2021 | 2021.08.14 | [GitHub](https://github.com/shuaiOKshuai/Tail-GNN) |
| ![Star](https://img.shields.io/github/stars/smufang/meta-tail2vec.svg?style=social&label=Star)<br>[**Towards locality-aware meta-learning of tail node embeddings on networks**](https://dl.acm.org/doi/10.1145/3340531.3411910) | CIKM 2020 | 2020.10.19 | [GitHub](https://github.com/smufang/meta-tail2vec) |
| [**Investigating and Mitigating Degree-Related Biases in Graph Convolutional Networks**](https://arxiv.org/abs/2006.15643) | CIKM 2020 | 2020.06.28 | - |

#### Unsupervised learning

| Title | Venue | Date | Code |
| - | - | - | - |
| ![Star](https://img.shields.io/github/stars/BUPT-GAMMA/Uncovering-the-Structural-Fairness-in-Graph-Contrastive-Learning.svg?style=social&label=Star)<br>[**Uncovering the Structural Fairness in Graph Contrastive Learning**](https://arxiv.org/abs/2210.03011) | NeurIPS 2022 | 2022.10.06 | [GitHub](https://github.com/BUPT-GAMMA/Uncovering-the-Structural-Fairness-in-Graph-Contrastive-Learning) |

### Topology imbalance

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Topology Uncertainty Modeling For Imbalanced Node Classification on Graphs**](https://ieeexplore.ieee.org/abstract/document/10094813) | ICASSP 2023 | 2023.05.05 | - |
| [**TopoImb: Toward Topology-level Imbalance in Learning from Graphs**](https://openreview.net/forum?id=nR3rZ4ODtQ) | LOG 2022 | 2022.11.23 | - |
| ![Star](https://img.shields.io/github/stars/RingBDStack/PASTEL.svg?style=social&label=Star)<br>[**Position-aware Structure Learning for Graph Topology-imbalance by Relieving Under-reaching and Over-squashing**](https://arxiv.org/abs/2208.08302) | CIKM 2022 | 2022.08.17 | [GitHub](https://github.com/RingBDStack/PASTEL) |
| ![Star](https://img.shields.io/github/stars/victorchen96/ReNode.svg?style=social&label=Star)<br>[**Topology-Imbalance Learning for Semi-Supervised Node Classification**](https://arxiv.org/abs/2110.04099) | NeurIPS 2021 | 2021.10.08 | [GitHub](https://github.com/victorchen96/ReNode) |

## Edge-level imbalance

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Edge Classification on Graphs: New Directions in Topological Imbalance**](https://arxiv.org/abs/2406.11685) | arXiv 2024 | 2024.06.17 | - |

## Graph-level imbalance

### Graph classification

| Title | Venue | Date | Code |
| - | - | - | - |
| ![Star](https://img.shields.io/github/stars/Puhongshan/BalanceGCL.svg?style=social&label=Star)<br>[**Graph Contrastive Learning with Balanced Hard Negatives and Fine-grained Semantic-aware Positives**](https://doi.org/10.1609/aaai.v40i29.39674) | AAAI 2026 | 2026.03.14 | [GitHub](https://github.com/Puhongshan/BalanceGCL) |
| ![Star](https://img.shields.io/github/stars/ALWAYS1815/iclr_UniImb.svg?style=social&label=Star)<br>[**One for Two: A Unified Framework for Imbalanced Graph Classification via Dynamic Balanced Prototype**](https://openreview.net/forum?id=MraQM41SNS) | ICLR 2026 Oral | 2026.01.26 | [GitHub](https://github.com/ALWAYS1815/iclr_UniImb) |
| [**SamGoG: A Sampling-Based Graph-of-Graphs Framework for Imbalanced Graph Classification**](https://arxiv.org/abs/2507.13741) | arXiv 2025 | 2025.07.18 | - |
| [**Cluster-Guided Contrastive Class-Imbalanced Graph Classification**](https://doi.org/10.1609/aaai.v39i11.33298) | AAAI 2025 | 2025.04.11 | - |
| [**When Imbalance Meets Imbalance: Structure-driven Learning for Imbalanced Graph Classification**](https://dl.acm.org/doi/10.1145/3589334.3645629) | WWW 2024 | 2024.05.13 | - |
| [**Towards Long-Tailed Recognition for Graph Classification via Collaborative Experts**](https://arxiv.org/abs/2308.16609) | arXiv 2023 | 2023.08.31 | - |
| [**RAHNet: Retrieval Augmented Hybrid Network for Long-tailed Graph Classification**](https://dl.acm.org/doi/10.1145/3581783.3612360) | ACM MM 2023 | 2023.08.04 | - |
| ![Star](https://img.shields.io/github/stars/YuWVandy/G2GNN.svg?style=social&label=Star)<br>[**Imbalanced Graph Classification via Graph-of-Graph Neural Networks**](https://dl.acm.org/doi/10.1145/3511808.3557356) | CIKM 2022 | 2022.10.17 | [GitHub](https://github.com/YuWVandy/G2GNN) |

### Graph size imbalance

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Graph Size-imbalanced Learning with Energy-guided Structural Smoothing**](https://arxiv.org/abs/2412.17591) | WSDM 2025 | 2024.12.23 | - |
| ![Star](https://img.shields.io/github/stars/shuaiOKshuai/SOLT-GNN.svg?style=social&label=Star)<br>[**On Size-Oriented Long-Tailed Graph Classification of Graph Neural Networks**](https://dl.acm.org/doi/10.1145/3485447.3512197) | WWW 2022 | 2022.04.25 | [GitHub](https://github.com/shuaiOKshuai/SOLT-GNN) |

## Federated graph learning

| Title | Venue | Date | Code |
| - | - | - | - |
| [**Towards Federated Long-Tailed Graph Learning: An Energy-Guided Dual Decoupling Approach**](https://arxiv.org/abs/2606.24237) | arXiv 2026 | 2026.06.23 | - |
| [**GraphFedMIG: Tackling Class Imbalance in Federated Graph Learning via Mutual Information-Guided Generation**](https://arxiv.org/abs/2508.10471) | arXiv 2025 | 2025.08.14 | - |

## Multimodal learning

| Title | Venue | Date | Code |
| - | - | - | - |
| [**SaVe-TAG: LLM-Based Interpolation for Long-Tailed Text-Attributed Graphs**](https://arxiv.org/abs/2410.16882) | KDD 2026 | 2026 | - |
| [**LLM-Empowered Class Imbalanced Graph Prompt Learning for Online Drug Trafficking Detection**](https://arxiv.org/abs/2503.01900) | arXiv 2025 | 2025.02.28 | - |
| ![Star](https://img.shields.io/github/stars/graphprojects/CM-GCL.svg?style=social&label=Star)<br>[**Co-Modality Graph Contrastive Learning for Imbalanced Node Classification**](https://openreview.net/forum?id=f_kvHrM4Q0) | NeurIPS 2022 | 2022.09.15 | [GitHub](https://github.com/graphprojects/CM-GCL) |

## Citation

If you find this repository useful, please cite it as follows:

```bibtex
@misc{yan2023awesomeimbalancedgraphs,
  author       = {Liang Yan},
  title        = {Awesome Imbalanced Learning on Graphs},
  year         = {2023},
  howpublished = {\url{https://github.com/yanliang3612/awesome-imbalanced-learning-on-graphs}},
  note         = {GitHub repository}
}
```

## Contributing

Contributions are welcome. To add a paper or code release, open a pull request or
an issue and include its title, venue, publication date, paper link, and code link
when available. Please place new entries in the most relevant category and order
them from newest to oldest.

## Contact

[Liang Yan](https://divinyan.com) · [yanliangfdu@gmail.com](mailto:yanliangfdu@gmail.com)
