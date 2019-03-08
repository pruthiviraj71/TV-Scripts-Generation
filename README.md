# TV Scripts Generation
[![Build Status](https://travis-ci.org/pruthiviraj71/TV-Scripts-Generation.svg?branch=master)](https://travis-ci.org/pruthiviraj71/TV-Scripts-Generation)

Building a Recurrent Neural Network to generate new scripts for Simpsons TV show.

## Requirements

- Tensorflow
- GPU for training (or Google Colaboratory for training purposes)

## Implementation

### Preprocessing

1. Lookup Table (Transformation of the words to ids to create a word embedding)
2. Tokenize Punctuation (To Implement the function token_lookup to return a dict that will be used to tokenize symbols like "!" into "||Exclamation_Mark||")

### Building the Neural Network

To build the neural network we implemented the following functions:
1. get_inputs
2. get_init_cell
3. get_embed
4. build_rnn
5. build_nn
6. get_batches

## Training

Result after 100 Epochs

![](https://github.com/pruthiviraj71/TV-Scripts-Generation/blob/master/training.png)

## Result

![](https://github.com/pruthiviraj71/TV-Scripts-Generation/blob/master/result.png)

```
Of course, The TV script doesn't make any sense. We trained on less than a megabyte of text. In order to get 
good results, We have to use a smaller vocabulary or get more data.
```
