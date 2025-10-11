# TFGA-Net
Pytorch implementation on: TFGA-Net: Temporal-Frequency Graph Attention Network for Brain-Controlled Speaker Extraction

## Introduction
The rapid development of auditory attention decoding (AAD) based on electroencephalography (EEG) signals offers the possibility EEG-driven target speaker extraction.However, how to effectively utilize the target-speaker common information between EEG and speech remains an unresolved problem. In this paper, we propose a model for brain-controlled speaker extraction, which utilizes the EEG recorded from the listener to extract the target speech. In order to effectively extract information from EEG signals, we derive multi-scale time--frequency features and further incorporate cortical topological structures that are selectively engaged during the task. Moreover, to effectively exploit the non-Euclidean structure of EEG signals and capture their global features, the graph convolutional networks and self-attention mechanism are used in the EEG encoder. In addition, to make full use of the fused EEG and speech feature and preserve global context and capture speech rhythm and prosody, we introduce MossFormer2 which combines MossFormer and RNN-Free Recurrent as separator.
Experimental results on both the public Cocktail Party and KUL dataset in this paper show that our TFGA-Net model significantly outper-forms the state-of-the-art method in certain objective evaluation metrics. Our codes and models will be available on GitHub after review.

<img width="1814" height="474" alt="image" src="https://github.com/user-attachments/assets/d2213602-0234-4a89-9944-7a54e148a51a" />


<p align="center">
  <img width="450" alt="image" src="https://github.com/user-attachments/assets/e588ca05-9002-490f-a601-38f1d75c0800" />
</p>


## Requiements
Python : 3.9.23

torch 2.5.1+cu118

## Datasets
The source and processing of the Cocktail Party dataset can be obtained [here](https://github.com/jzhangU/Basen)

KUL dataset can be obtained [here](https://zenodo.org/records/4004271)

## Code Availability
The training logs in this paper are available in the train_logs.txt.

The core source code for reproducing our results are available in the TFGA-NET.ipynb
