# MMFedEKT
# Implementation for Embedding Knowledge Transfer for Multimodal FL

======

This repository implements all experiments for knowledge transfer in multimodal FL

Abstract
======
Federated learning (FL) enables a decentralized machine learning paradigm for multiple clients to collaboratively train a generalized
global model without sharing their private data. Most existing works have focused on designing FL systems for unimodal data,
limiting their potential to exploit valuable multimodal data for future personalized applications. Moreover, the majority of FL
approaches still rely on labeled data at the client side, which is often constrained by the inability of users to self-annotate their
data in real-world applications. In light of these limitations, we propose a novel multimodal FL framework, namely FedMEKT,
based on a semi-supervised learning approach to leverage representations from different modalities. To address the challenges of
modality discrepancy and labeled data constraints in existing FL systems, our proposed FedMEKT framework comprises local
multimodal autoencoder learning, generalized multimodal autoencoder construction, and generalized classifier learning. Bringing
this concept into the proposed framework, we develop a distillation-based multimodal embedding knowledge transfer mechanism
which allows the server and clients to exchange joint multimodal embedding knowledge extracted from a multimodal proxy dataset.
Specifically, our FedMEKT iteratively updates the generalized global encoders with joint multimodal embedding knowledge from
participating clients through upstream and downstream multimodal embedding knowledge transfer for local learning. Through
extensive experiments on three multimodal human activity recognition datasets, we demonstrate that FedMEKT not only achieves
superior global encoder performance in linear evaluation but also guarantees user privacy for personal data and model parameters
while demanding less communication cost than other baselines.

Data
=====
**Data can be downloaded at: https://drive.google.com/drive/folders/1u101j5PYkDq6E65QimpWOBgBSDo2Kabp?usp=sharing**

Running Instruction
=====

**Environment:** Python 3.8, pytorch

**Main File:** FedMEKT_main.py

**Modify parameters setting in `Setting.py` to run the code**

----------

**To run the code, use the command in terminal**:
```
python FedMEKT_main.py
```










