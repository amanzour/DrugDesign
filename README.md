# DrugDesign

LSTM Recurrent Neural Networks are specially effective in learning small molecule representations and exploring the molecular space by generating candidate molecules most of which have correct SMILES representation.
Here, we use Deep Learning to explore the molecular space and  generate new small molecules from the already observed ones.
The procedure and codes closely follow Cheminformania. See https://www.cheminformania.com/master-your-molecule-generator-seq2seq-rnn-models-with-smiles-in-keras/ for full details.
Prodecure is as follows:
First, we download a set of small molecules from GDB https://gdb.unibe.ch/downloads/.
We then, use the SMILES format of the molecules to convert them to numerical vectors
Then, using an LSTM RNN, we train the network to predict the next character of the SMILES representation of a small molecule by having observed previous ones.
We finally show that we can use the latent stage of the neural network to generate different predictions or molecules.  
