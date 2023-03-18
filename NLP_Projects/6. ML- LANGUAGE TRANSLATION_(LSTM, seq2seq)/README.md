# <b> PROJECT :Character-level Language Translation using LSTM-based Seq2Seq Model
_____________________

## OBJECTIVE:
  > The aim is to implement a character-level sequence-to-sequence model, processing the input 'character-by-character' and generating the output 'character-by-character' (English ----> FRENCH).
  
## PROJECT WALKTHROUGH :
  >* Data preprocessing: The English and French sentence pairs are preprocessed by tokenizing the sentences and converting them into sequences of integers. The sequences are then padded to have equal length.
  >* One-hot vectorization: The preprocessed sequences are one-hot vectorized to create three NumPy arrays: encoder_input_data, decoder_input_data, and decoder_target_data. The encoder_input_data is a 3D array of shape (num_pairs, max_english_sentence_length, num_english_characters), while decoder_input_data and decoder_target_data are 3D arrays of shape (num_pairs, max_french_sentence_length, num_french_characters).
  >* Model training: A basic Seq2Seq LSTM model is trained using teacher forcing. The model takes encoder_input_data and decoder_input_data as inputs and predicts decoder_target_data.
  >* Model deployment: The trained model can be used to translate new English sentences into French. The English sentence is first preprocessed and one-hot vectorized, and then fed into the trained model to generate the corresponding French sentence.

## TECHNOLOGIES/LIBRARIES USED:
  >* Python
  >* Numpy
  >* Sklearn
  >* Tesnsorflow
  >* Keras
  
## HOW TO RUN:
  > To run this code, follow these steps:

  >* Clone this GitHub repository.
  >* Open the notebook machine_learning_language_translation.ipynb in Jupyter Notebook or Google Colab.
  >* Follow the instructions provided in the notebook to run each code cell in the correct order.
  
  
## License:
This project is licensed under the MIT License.
