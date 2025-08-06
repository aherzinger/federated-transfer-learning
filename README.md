# Federated Transfer Learning
This repository provides a notebook that uses a simple FTL approach, using a pretrained model (Resnet-18) and use FTL to further train it on recognizing pictures of the CIFAR-10 Dataset. This transfers the knowledge of the pretrained model to a new domain (Resnet-18 was pretrained on ImageNet Dataset). Furthermore we showcased how much different Non-IID Data Distributions affect performance and effectiveness of this approach, as well as how these Data Limitations can be adressed by using different FL-Strategies.
## Main ideas and definitations
### Definiton Federated Learning

Federated Learning (FL) is a decentralized machine learning paradigm where multiple entities collaborate to train a model without sharing their raw data. Each participant trains a local model on their private data and shares only model updates (e.g., gradients) with a central server, which aggregates these updates to build a global model. This approach addresses data privacy concerns and leverages distributed data sources. 

### Definition Transfer Learning

Transfer Learning (TL) involves leveraging knowledge gained from one task to improve learning performance in a different but related task. Instead of training a model from scratch, TL utilizes pre-trained models on large datasets and fine-tunes them for specific target tasks, especially when labeled data is scarce. 

### Definition FTL

Federated Transfer Learning (FTL) combines the principles of FL and TL to enable collaborative model training across decentralized datasets with different feature spaces or distributions while preserving data privacy. FTL is particularly useful when participants have heterogeneous data and seek to benefit from shared knowledge without compromising sensitive information.


