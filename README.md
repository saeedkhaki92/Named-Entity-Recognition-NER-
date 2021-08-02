# Named-Entity-Recognition-NER
Named Entity Recognition is a subtask of information extraction that locates and classifies named entities in a text. The project uses Trax deep learning library for implementation.

An NER example is as follows: 

![Alt Text](https://github.com/saeedkhaki92/Named-Entity-Recognition-NER-/blob/main/ner.png)

## Getting Started

### Dependencies

Following packages should be installed on python 3:

- Trax
- numpy
- random


<a href="https://github.com/google/trax" target="_blank">Trax</a> is an end-to-end library for deep learning that focuses on clear code and speed. It is actively used and maintained in the Google Brain team. It is faster than Tensorflow and Pytorch and also the codes are more clear. It also supprts both TPUs and GPUs.


## Dataset

We will be using a dataset from Kaggle, which we will preprocess for you. The original data consists of four columns, the sentence number, the word, the part of speech of the word, and the tags. A few tags you might expect to see are:

- geo: geographical entity
- org: organization
- per: person
- gpe: geopolitical entity
- tim: time indicator
- art: artifact
- eve: event
- nat: natural phenomenon
- O: filler word

## Model

The model architecture will be as follows:


![Alt Text](https://github.com/saeedkhaki92/Named-Entity-Recognition-NER-/blob/main/ner2.png)



- We use the input tensors you built in your data generator
- Feed it into an Embedding layer, to produce more semantic entries
- Feed it into an LSTM layer
- Run the output through a linear layer
- Run the result through a log softmax layer to get the predicted class for each word.




## Instructions

You can train the model from scrath using the Google Colab notebooks. Please use `NER_trax.ipynb` for Trax version.

## Results

I trained the model for several epochs and the validation accuracy is around 95%.

