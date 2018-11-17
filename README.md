# CRF-bi-LSTM-sequence-tagging-Chinese-characters-
&emsp;&emsp;We use Python3.6+tensorflow1.12.0 to coding the bi-LSTM+CRF network structure and realizing the sequence tagging for chinese characters.

&emsp;&emsp;(1)Raw data propecessing. Calling ` ` `vocab_build()` ` ` function to convert the data of .txt format to .pkl format. And initilazing the word vectors.(We set the dinmension of vectors is 300)

&emsp;&emsp;(2)Designing the network structure and hyper-parameters, calling ` ` `main.py` ` ` train and test model.

- batch_size=64;
- epoch=25;
- learning_rate=0.001;
- dropout=0.5;
- gradient_clipping=5.0;
- LSTM_num(forward)=300;
- LSTM_num(backward)=300；
- optimizer=Adam;
- ...

&emsp;&emsp; After 25 epoch, the precision, recall, F1 values of test set as shoun below.

<center>

![Results](results.png)
<br/>
Fig. precision, recall, F1 values
</center>

- precision=0.951266;
- recall=0.908613;
- f1=0.929270.
(After 25 iterations)