# NLP_models_benchmarks_on_IMDB_dataset


This REPO is for assessing multiple NLP models architecture on a sentiment analysis task using IMDB reviews dataset .

![image](https://user-images.githubusercontent.com/85687148/128555608-c8143fbd-6e7a-4f48-b561-08138f9e2400.png)


<a href="https://ai.stanford.edu/~amaas/data/sentiment/"> ***IMDB Sentiment Analysis*** </a> : This is a dataset for binary sentiment classification containing substantially more data than previous benchmark datasets. We provide a set of 50,000 highly polar movie reviews for training and testing, each review has a binary label corresponding to 0 for negative Sentiment and 1 for a positive sentiment.
This is how the data head looks like :

<p align="center">
  <kbd>
  <img width="460" height="250" src="https://user-images.githubusercontent.com/85687148/128259390-89679a0d-629a-49fe-a97d-bd988cf0a4f0.png">
  </kbd>
</p>
  
  
  
## Results :

For each model we have the following architecture and test accuracy :

  <table>
        <thead>
            <tr>
                <th>Rank</th>
                <th>Model</th>
                <th>Test Accuracy </th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>BERT + Dropout Layer + Fully Connected Layer + Sigmoid</td>
              <td><b>92%</b></td>
            </tr>
            <tr>
                <td>2</td>
                <td>
                    <p>TF-IDF + Logistic Regressor Classifier</p>
                    <p>TF-IDF + SVM Classifier</p>
                </td>
                <td>89%</td>
            </tr>
            <tr>
                <td>3</td>
                <td>DOC2VEC + Dropout Layer + Fully Connected Layer + Sigmoid</td>
                <td>80%</td>
            </tr>
            <tr>
                <td>4</td>
                <td>DOC2VEC + BiLSTM + Dropout Layer + Fully Connected Layer + Sigmoid</td>
                <td>78%</td>
            </tr>
        </tbody>
    </table>

