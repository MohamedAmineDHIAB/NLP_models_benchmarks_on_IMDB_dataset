# Fine-Tuning BERT on IMDB Dataset :


<p align="center">
  <kbd>
  <img width="460" height="300" src="https://user-images.githubusercontent.com/85687148/128644652-26320c24-8745-44f5-beaa-d9a16995bc34.png">
  </kbd>
</p>


## ***Requirements*** :

* Pandas
* Seaborn
* Matplotlib
* Pytorch
* transformers==3
* numpy
* collections

## ***Testing the Model without training*** :

**Uncompress the pre-trained model using :**

`cat compressed_model.gz* | zcat > best_model_state.bin`

**Import it in your Python script using :**


`model = SentimentClassifier(len(class_names))`

`model.load_state_dict(torch.load('best_model_state.bin'))`

`model = model.to(device)`


## ***Training the Model*** :


`Epoch 1/2
Train loss 0.316 accuracy 0.888
Val   loss 0.283 accuracy 0.914`

`Epoch 2/2
Train loss 0.182 accuracy 0.955
Val   loss 0.355 accuracy 0.920`

`CPU times: user 1h 13min 5s, sys: 4min 6s, total: 1h 17min 12s
Wall time: 1h 17min 14s`


## ***Testing the Model*** :


`
Model Test Accuracy :   0.921
`
## ***Confusion Matrix***


<p align="center">
  <kbd>
  <img width="460" height="300" src="https://user-images.githubusercontent.com/85687148/128558564-c6dc1640-5bc0-466d-883d-89b4e8c9e929.png)">
  </kbd>
</p>




