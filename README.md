# Clustering-South_German_Credit_Data

About The dataset:
Häußler (1979, 1981) and Fahrmeir and Hamerle (1981, 1984) gave an account on the story behind the data, which is summarized here: the data are a stratified sample of 1000 credits (300 bad ones and 700 good ones) from the years 1973 to 1975 from a large regional bank in southern Germany, which had about 500 branches, among them both urban and rural ones.
Bad credits are heavily oversampled, in order to acquire sufficient information for discriminating them from good ones; the sources report that the actual prevalence of bad credits is around 5%; thus, in a Bayesian context, 5% might be used as a prior probability for a credit being bad.
As suggested with the Statlog German credit data, one might consider misclassification cost, and it has been suggested to allocate the cost for misclassifying a bad risk as good to be five times as high than the cost for misclassifying a good risk as bad. 
The credits are part of normal bank business, i.e. all debtors must have passed some checks of creditworthiness before being granted the credit; this, of course poses a severe limitation for the usability of the data in support of credit decisions for general requests (as was also noted e.g. by Häußler 1979). 
According to Fahrmeir and Hamerle (1984), customers with “good” credits perfectly complied with the conditions of the contract while customers with “bad” credits did not comply with the contract as required.

Approach the problem: 
This is a classification problem, but instead I used the dataset to find groupings through K-means clustering. I grouped debtors using K-means clustering so that there are distinct groups corresponding to those who are "bad" credits vs those who are "good." As thhis is an unsupervised problem, I did not use the target column for clustering. I just used the atrget column for checking the accuracy of the cluster.
But, using the target values after clustering, compute the percentage of good credit ("1" in the target column) vs bad credit ("0" in the target column) for each group and your overall accuracy of prediction using clustering.
