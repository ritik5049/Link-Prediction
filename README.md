# Link Prediction using Machine Learning


## Introduction
The social network graph is a graph that represents social relations between entities. It is a model or representation of a social network. As in the graph, the nodes here represented as each individual and the connection between them(link) represented as the social relation(friendship, follower-followee relation etc). The social graph has been referred to as “the global mapping of everybody and how they’re related”.

![social.jpeg](https://miro.medium.com/max/875/1*f_S71NTnTWueN4tDJt6UPA.jpeg)

## Dataset
The dataset from the Stanford Large Network Dataset Collection. The dataset is reasonably sized with 7126 nodes. The total number of possible edges in the network is 50,772,750  from which 35,324 are present in the network. The dataset is highly skewed thus sampled 35,324 edges and labelled them as missing link.

## Feature Extraction
Used the 70,648 edges to extract variou features such as- 
* Page Rank
* Shortest  Path 
* Follower  &  Followee  Counts 
* Inter/Common  Followers  &  Followee  Counts

![Screenshot 2021-08-01 210815](https://user-images.githubusercontent.com/52758299/127776836-d692f824-a937-419b-9bf9-7cc2b3599aca.jpg)

## Model Building 
Standardisation of data - features  like number of followers  have  a  wider  distribution than  page rank  because  of  which number of followers  will  dominate  over page rank, thus we standardised the data. Training  and  Testing set were spllited 70% data as training set and 30% as test set. For the classification  problem,  we have  trained  three  models  namely,  Logistic Regression, Random Forest, Support Vector Machine.

## Logistic Regression: Precision = 92%, Recall = 98%, Accuracy= 95%
![image](https://user-images.githubusercontent.com/52758299/127777112-6cbe8cf1-3fd7-4019-8c57-d74fd32731ce.png)
![image](https://user-images.githubusercontent.com/52758299/127777116-e3025bd3-6504-4ff7-9108-192e282a60db.png)


## Random Forest: Precision = 96%, Recall = 98%, Accuracy= 97%
![image](https://user-images.githubusercontent.com/52758299/127777145-cd310342-8bad-41df-88cc-e7f2f0e25e78.png)
![image](https://user-images.githubusercontent.com/52758299/127777146-70045669-521d-4145-b69a-de561f482d05.png)


## Support Vector Machine(SVM): Precision = 93%, Recall = 97%, Accuracy= 95%
![image](https://user-images.githubusercontent.com/52758299/127777171-824e5738-c5a6-48ac-8cd4-66fb881e2b7d.png)
![image](https://user-images.githubusercontent.com/52758299/127777177-49f34ddf-29c4-483b-9386-ddf4c0c1116e.png)

## ROC Curve

![Screenshot 2021-08-01 212112](https://user-images.githubusercontent.com/52758299/127777235-943a2d79-7974-4233-927e-01e61f836ec0.jpg)








