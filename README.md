Convolutional Recurrent Neural Network (CRNN) Implement with pytorch for chinese OCR.

1. Prepare training data, you can find samples(with labels) in the folder of "data", it looks like:


![Alt text](https://github.com/dcrmg/CRNN_OCR_pytorch/blob/master/data/07909298-5a3f-11e8-a408-000c29cf3ddc.jpg)

![Alt text](https://github.com/dcrmg/CRNN_OCR_pytorch/blob/master/data/08df0480-5a3f-11e8-a408-000c29cf3ddc.jpg)


2. Create LMDB database
   cd create_dataset
   python  create_dataset.py

3. train CRNN for chinese OCR
   cd pytorch-train
   python crnn_main.py --cuda

you can find trained model in the folder of "save_model"


notes:
   1. needs to be carefully confirmed whether your Chinese characters are in alphabet or not.
   2. good performance in training accuracy, and bad performance in practical application? maybe  samples of various situations are needed.
