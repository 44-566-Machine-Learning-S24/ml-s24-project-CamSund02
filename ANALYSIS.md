# ANALYSIS

# Links
[Models Notebook](Notebooks\Models.ipynb)\
[Link to next markdown file DATA.md](CONCLUSIONS.md)
## Metrics
### Linear Regression
Test R^2 Score: 0.68\
Test Root Mean Squared Error: 218441.55
### K-means PCA
Distortion: 221592391.13\
Silhouette Score: 0.65
### K-means 2d
Distortion: 8608765190229.747\
Silhouette Score: 0.60
### Decision Tree
Test Accuracy: 0.492\
Test F1 Score: 0.043
### Linear SVM
Test Accuracy: 0.000\
Test F1 Score: 0.000
### RBF SVM
Test Accuracy: 0.000\
Test F1 Score: 0.000
### Polynomial SVM
Test Accuracy: 0.000\
Test F1 Score: 0.000
### Sigmoid SVM
Test Accuracy: 0.000\
Test F1 Score: 0.000
### Stochastic Gradient Descent
Test Accuracy: 0.000\
Test F1 Score: 0.000
### Random Forest
Test Accuracy: 0.041\
Test F1 Score: 0.037
### Neural Net
Test Accuracy: 0.008\
Test F1 Score: 0.001

For Random Forest and Decision Tree I tuned them by changing their max depth values to see if the results would get better. All results can be found in [Models Notebook](Notebooks\Models.ipynb). A challenge that I faced was that since I was using 1 notebook for all my models variables were getting reused and were changing, making some of my results different from what they should be. I fixed this by making each model their own variables set to their specific name.

Another challenge was getting my K-means clustering to look correct, initially I was doing it wrong by splitting the data into train and test splits but after the K-means assignment I ended up putting all my features together and seeing what I got out of that.

A limitation on my results that was a big issue was the number of features I had available. Since I scraped Zillow and didn't use a premade dataset I didn't have access to many features. I think that if I had more things to base my model on I could have gotten much better numbers for my models.\
Some improvements that could be made would be getting more and better feautes and with those extra features trying new dimensional reducations and seeing if I could get my accuracy's much higher.
