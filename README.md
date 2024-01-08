# Ciphertext-decryption-for-any-keys-
The purpose of this project is to create an LSTM model that given a string encoded using Caesar’s Cypher breaks the code and receieves the original string! 
This is how we approached the question
* First we created a dataset with random 5000 sentences and their encrypted text
using a random key from 1 to 25. The aim of this lstm was to break any key used for
encryption

*The next step was to tokenize the data and convert both plaintext and ciphertext
into vectors and pad them adequately

*Then we constructed an LSTM architecture. We specifically used an attention
layer as mentioned in an original research paper for better and accurate results.

*This approach can work because it uses a sequential structure with LSTM layers,
known for their ability to capture sequential patterns effectively. The embedding
layer helps translate tokens into meaningful vector representations, while batch
normalization and dropout enhance training stability and prevent overfitting. The
presence of a custom attention mechanism suggests a potential for focusing on
relevant parts of the input during decoding. The model employs large hidden units in
its LSTM layers, which can capture complex patterns. The softmax activation in the
final layer is well-suited for generating sequences

*The model was then compiled using a custom sequence to sequence loss

*The model was trained and then tested. 

* Our model worked reasonably well giving great evaluation metrics including accuracy of 96.95% and an F1 score of 0.93.
 *This project showcases promising results in using ML in security related practices such as encryption algorithm. 



