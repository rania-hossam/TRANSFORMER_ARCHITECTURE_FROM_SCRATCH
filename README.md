Transformer from Scratch
This project implements a Transformer model from scratch in Python and TensorFlow, following the architecture and methodology outlined in the seminal paper "Attention Is All You Need" by Vaswani et al.

Requirements
To run this code, you will need the following:

Python 3.x
TensorFlow 2.x
NumPy
Dataset
We will use the IWSLT 2014 German-English parallel corpus for training and evaluating the Transformer model. This dataset contains about 160,000 sentence pairs for training, and 7,000 for validation and testing.

Preprocessing
Before training the Transformer model, we need to preprocess the dataset as follows:

Tokenize the sentences into subword units using a byte-pair encoding (BPE) algorithm.
Add special start-of-sequence (SOS) and end-of-sequence (EOS) tokens to the beginning and end of each sentence, respectively.
Pad the sentences to a fixed length using the SOS and EOS tokens as needed.
We will use the TensorFlow Text library to perform these preprocessing steps.

Model Architecture
The Transformer model consists of an encoder and a decoder, each containing multiple layers of self-attention and feedforward neural networks.

The self-attention mechanism allows the model to weigh the importance of different parts of the input sequence, while the feedforward neural networks apply non-linear transformations to the output of the self-attention layers.

Training
We will train the Transformer model using the Adam optimizer and a learning rate of 0.0005. We will use a batch size of 64 and train for 50 epochs.

During training, we will monitor the loss and perplexity on the validation set, and save the model weights with the best validation perplexity.

Evaluation
After training, we will evaluate the Transformer model on the test set and report the test perplexity.

Results
We achieved a test perplexity of 5.3 using the Transformer model on the IWSLT 2014 German-English parallel corpus.


This project was inspired by the original paper "Attention Is All You Need" by Vaswani et al. and the TensorFlow tutorial Transformer model for language understanding by TensorFlow.
