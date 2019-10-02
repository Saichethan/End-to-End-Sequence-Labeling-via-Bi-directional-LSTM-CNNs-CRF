# NERmultimodal
## 1.Introduction 
Keras Implementation of "End-to-end Sequence Labeling via Bi-directional LSTM-CNNs-CRF" by Ma Hovy et al 2016, on multimodal dataset from "Adaptive Co-attention Network for Named Entity Recognition in Tweets" paper AAAI 2018. Different datasets can be used. 

## 2. Requirements
1) Python 2.7 or higher
2) Keras 1.2 (the vesion including the CRF model), the backend is theano.
3) Moreover, you need to download the word embedding trained by tweets from http://pan.baidu.com/s/1boSlljL. 

## 3. Data Format
Our datasets include 8,257 tweet and image pairs. We split the dataset into three parts: the training set, development set, and testing set, which contain 4,000, 1,000, and 3,257 tweets, respectively.  
      

IMGID:418340        
Rep	O        
.	O        
Howard	B-PER        
Coble	I-PER        

## 4. Usage
Preprocess datasets accordingly(for other datasets)
1) Training the model:
	$ python CNN_BiLSTM_CRF.py

## 5. Evalution
The Evaluation code to calculate F1, Precision, and recall is in ner_evaluate.py. 


