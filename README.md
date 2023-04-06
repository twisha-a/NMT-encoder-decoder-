# NMT-encoder-decoder-
Create an LSTM encoder-decoder model that will translate English sentences into French using Encoder-Decoder LSTM.
## Steps followed
1. **Importing Libraries**
2. **Dataset** - The dataset contains English sentences and their French translations. ![Dataset Link](http://www.manythings.org/anki/)
3. **Data Preprocessing** - Generated two copies of the translated sentence: one with the start-of-sentence token and the other with the end-of-sentence token.
4. **Tokenization and Padding** - tokenizing the original and translated sentences and applying padding to the sentences that are longer or shorter than a certain length as LSTM expects an equal length for all the inputs
5. Word Embeddings - For English sentences, i.e. the inputs, we will use the GloVe word embeddings. For the translated French sentences in the output, we will use custom word embeddings. And then create an embedding Layer for the LSTM Model.
6. Create the Model - Now we define our outputs with the length of our output sentence as 12. The final layer of the model will be a dense layer, therefore we need the outputs in the form of one-hot encoded vectors, since we will be using softmax activation function at the dense layer. Next, we need to create the encoder and decoders. The input to the encoder will be the sentence in English and the output will be the hidden state and cell state of the LSTM.
7.
8.
