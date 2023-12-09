## Bi-LSTM based Poetry and Text Generation

NLP techniques using the RNN variant, LSTM (Long Short-term Memory) for text and poetry generation using the right-to-left and left-to-right bidirectional techniques.

# Improvisation Under Progress
Implementation of the same use case using SOTA transformers (work under progress)

# Preprocessing Techniques
<ul>
  <li>Sentence Tokenisation</li>
  <li>Sentence N-Gram Sequencing</li>
  <li>Sequence Padding</li>
  <li>One-hot Encoding (Categorical Encoding)</li>
</ul>

# Model Architecture
Tensorflow based implementation of a sequential model consisting of these hidden layers:
<ul>
  <li>Embedding Layer</li>
  <li>Bidirectional LSTM Layer</li>
  <li>Dense Output Layer</li>
</ul>

# Prediction
An input prompt, also called a seed is provided to the model. This is run over a `for` loop for the word count and subsequent words are predicted. <br>

In each loop:
<ul>
  <li>Converion of seed to sequence</li>
  <li>Padding of the sequences</li>
  <li>Prediction of the probabilities of next word using the padding sequence</li>
  <li>Conversion of the predicted index to word from the token dictionary</li>
  <li>Appending the obtained word to the seed</li>
</ul>

# Final Comments
This simple project was done to understand NLP Preprocessing and Modelling Techniques in depth, as a part of Coursera's course <a href="https://www.coursera.org/learn/natural-language-processing-tensorflow">Natural Language Processing in TensorFlow</a>.
<br>
Thanks for stopping by! Happy Coding :))
