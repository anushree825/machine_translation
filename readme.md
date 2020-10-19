# Data
Note that the preprocessing is different for punctuation and without punctuation

If the data is in a csv file, use the data prep part of the code.
If the data has 4 files (src_train.src, trg_train.trg, src_test.src, trg_test.trg)

# Specify the parameters as shown below:

d = Dataset(source_files, target_files, batch_size=10)
embedding_dim = 50
hidden_dim = 100 
num_layers = 4 (Num of layers for LSTM)

# Run the following to 'train and save model' for 'Seq to Seq'

train_and_save(m, d, "seq2seq_")

# Run the following to 'train and save model' for 'Seq to Seq with Attention'

train_and_save(m, d, "attention_")

# Run the following to 'train and save model' for 'Seq to Seq - No punct'

train_and_save(m, d, "seq2seq_noPunc_")

# Run the following to 'train and save model' for 'Seq to Seq with Attention - No punct'

train_and_save(m, d, "attention_noPunc_")