# Word to Phoneme Converter

## Word Pronunciations: Word to Phoneme Conversion

<div class='alert alert-info'><strong>Phoneme Conversion:</strong> Converts lexical orthographic symbols (words) to phonetic representation along with other possible information such as stress placement.</div>


### Phoneme Conversion
- Words to phonemes converters can help you figure out how to pronounce a certain word. e.g. Google word pronunication utility
- Conversion of words to phonemes is an important step in the process of Text-to-Speech synthesis, where a system is given an input text which is preprocessed through various stages to identify how a text sentence needs to be spoken out loud by identifying the pronunciations and prosody of each word present in the sentence. 

### Encoder-Decoder Architecture
- This type of architecture can be used for solving Sequence to Sequence problems aka Seq2Seq
- Seq2Seq encoder decoder architectures can be constructed using the Recurrent Neural Networks (RNNs) (Transformers being a more popular choice these days)
- LSTM, which is a variant of RNN, will be used in this kernel
- This architecture is comprised of two models: one for reading the input sequence and encoding it into a fixed-length vector, and a second for decoding the fixed-length vector and outputting the predicted sequence.
- We can formulate the problem of word to phoneme conversion in the same way, where the words are tokenized at a character level and passed as an input sequence of fixed length to the encoder, and the decoder is supposed to predict the output sequence of phonemes.
- This kind of architecture is/was (Transformers have overtaken) typically used in language translation models, where a sentence in one language is passed as an input sequence to the decoder and the encoder predicts the output sequence in the target language.

![This is an image](https://i.imgur.com/vzkiAnZ.png)

## Pipeline
1. Data Preparation
2. Preprocessing
3. Modelling
4. Model Inference

## Python Libraries Required
```
pip install numpy
pip install pandas
pip install matplotlib
pip install seaborn
pip install tensorflow
```



