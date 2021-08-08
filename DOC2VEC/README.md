# Fine-Tuning BERT on IMDB Dataset :

## ***Requirements*** :

* Python 2:
  * Pandas
  * gensim
  * numpy
  * nltk
  * tqdm
  * Matplotlib

* Python 3:
  * Pandas
  * Seaborn
  * Matplotlib
  * Pytorch with CUDA support
  * numpy
  * tqdm


## ***Getting the embeddings of the review texts using pre-trained Doc2Vec Model*** :

1- download the doc2vec pretrained weights from the google drive link <a href="https://drive.google.com/file/d/1813Css0589E6_SE-VJyW7GDaDiZNG2SR/view?usp=sharing">doc2vec.bin </a> and put the binary file in `./data/`
2- follow `embeddings_with_doc2vec.ipynb` to get a csv file containing a DataFrame with a column of the corresponding embeddings for each review.

## ***Training the Pytorch Neural*** :

  0%|          | 4/10000 [00:00<05:02, 33.03it/s]
  --------------------------------------------------
Epoch 0: train loss: 0.690

 30%|███       | 3006/10000 [01:14<02:49, 41.17it/s]
 --------------------------------------------------
Epoch 3000: train loss: 0.412

 60%|██████    | 6007/10000 [02:29<01:37, 40.96it/s]
 --------------------------------------------------
Epoch 6000: train loss: 0.371

 90%|█████████ | 9009/10000 [03:42<00:23, 41.52it/s]
 --------------------------------------------------
Epoch 9000: train loss: 0.354

100%|██████████| 10000/10000 [04:06<00:00, 40.54it/s]


## ***Testing the Model*** :


`
Model Test Accuracy :   0.800
`
## ***Confusion Matrix***

