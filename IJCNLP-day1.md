# Day1

## Words and People
Speaker: Rada Mihalcea, University of Michigan

* word association 
    * sleep: dream for young, awake for old
    * diffierence between gender and culture

## Grammatical Error Detection Using Error- and Grammaticality-Specific Word Embeddings
Masahiro Kaneko, Yuya Sakaizawa and Mamoru Komachi

* Bi-LSTM has highest accuracy
* W&GWE-L8 is slightly better than Word2Vec

## Dependency Parsing with Partial Annotations: An Empirical Comparison
Yue Zhang, Zhenghua Li, Jun Lang, Qingrong Xia and Min Zhang

* use stack and input queue

## Convolutional Neural Network with Word Embeddings for Chinese Word Segmentation
Chunqi Wang and Bo Xu

* Neural network sequence labeling models for Chinese Word Segmentaiton
* CNN is able to capture rich n-gram features effectively
* GLU as activation function instead of ReLU

## A Computational Study on Word Meanings and Their Distributed Representations via Polymodal Embedding
Joohee Park and Sung-Hyon Myaeng

* render charector into picture then inpu to CNN
* GRU
* n-gram model don't have much diffence in result
* 3-gram + radical + GloVe
* Slightly better than ZPar
* BiRNN-CRF for joint segmentiation 

# Day 2

## Reusing Neural Speech Representations for Auditory Emotion Recognition
Egor Lakomkin, Cornelius Weber, Sven Magg and Stefan Wermter

* speech dataset is not enough
* Conv layer and Recurrent layer

## Local Monotonic Attention Mechanism for End-to-End Speech And Language Processing
Andros Tjandra, Sakriani Sakti and Satoshi Nakamura


## Attentive Language Models
Giancarlo Salton, Robert Ross and John Kelleher

* attention weight spreads out across the history

# Day 3

## Estimating Reactions and Recommending Products with Generative Models of Reviews
Jianmo Ni, Zachary C. Lipton, Sharad Vikram and Julian McAuley

## Summarizing Lengthy Questions
Tatsuya Ishigaki, Hiroya Takamura and Manabu Okumura

* Copy Mechanism better

## Concept-Map-Based Multi-Document Summarization using Concept Coreference Resolution and Global Importance Optimization
Tobias Falke, Christian M. Meyer and Iryna Gurevych

* concept graph
* meteor and rouge-2
* supervised importance scoring 
* https://github.com/UKPLab/ijcnlp2017-cmaps

## Abstractive Multi-document Summarization by Partial Tree Extraction, Recombination and Linearization
Litton J Kurisinkel, Yue Zhang and Vasudeva Varma

* maximun density tree cut algorithm
* cluster partial tree (k_means)
* cluster graph for ILP
* ZGen framework for syntatic tree linearization

## Towards Abstractive Multi-Document Summarization Using Submodular Function-Based Framework, Sentence Compression and Merging
Yllias Chali, Moin Tanvee and Mir Tafseer Nayeem

## Dataset for a Neural Natural Language Interface for Databases (NNLIDB)
Florin Brad, Radu Cristian Alexandru Iacob, Ionel Alexandru Hosu and Traian Rebedea

* Natural Language interface to SQL
* carwled SQL from stackoverflow
* BLEU score 
* bad result in long query


## Proofread Sentence Generation as Multi-Task Learning with Editing Operation Prediction
Yuta Hitomi, Hideaki Tamori, Naoaki Okazaki and Kentaro Inui

* 330 articles / day and 2.5 times review / article
* generate proofread sentence on Attention based seq2seq but recall is low
* Seq2Seq + EOP got better result
* add learning rate to EOP
