Download Link: https://assignmentchef.com/product/solved-cs156-homework-3-classification
<br>
The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this assignment, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (i.e., name, age, gender, socio-economic class, etc.).




<strong>Overview</strong>

The dataset called Data-Hw3.csv consists of 891 entries. This dataset needs to be split into two groups using 25% data for Test set

The training set should be used to build your machine learning models. For the training set, we provide the outcome (also known as the “ground truth”) for each passenger. Your model will be based on “features” like passengers’ gender and class.




The test set should be used to see how well your model performs on unseen data. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.




The dataset for this project contains information about the passengers in the Titanic and if they survived the historic accident. There are 8 column headers:

<ol>

 <li>passenger ID An identifier for the passenger</li>

 <li>name Name of the passenger</li>

 <li>sex Male or Female</li>

 <li>age Age in years</li>

 <li>sibsp # of siblings / spouses aboard the Titanic</li>

 <li>parch # of parents / children aboard the Titanic</li>

 <li>pclass Ticket class. 1 = 1<sup>st</sup>, 2 = 2<sup>nd</sup>,  3 = 3<sup>rd</sup></li>

 <li>survived 0 = “no”, 1 = “yes”</li>

</ol>

<strong>Variable Notes</strong>

pclass: A proxy for socio-economic status (SES)1st = Upper2nd = Middle3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, it in the form of xx.5

sibsp: The dataset defines family relations in this way…Sibling = brother, sister, stepbrother, stepsisterSpouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way…Parent = mother, fatherChild = daughter, son, stepdaughter, stepsonSome children travelled only with a nanny, therefore parch=0 for them.

<strong> </strong>

<strong><u> </u></strong>

<strong><u>Part (A):</u></strong> Data Import, Data Pre-processing

<ol start="3">

 <li>Read the file Data-Hw3.csv</li>

 <li>Replace Missing Data to make the data set complete</li>

 <li>Divide the data set into Training set and Test set</li>

</ol>




For each model in Parts (B) through (H), use the following data set to test your model:

<strong><u> </u></strong>

<strong><u>Data set to test your models:</u></strong>

<ol>

 <li>[sex = male, age = 4, sibsp = 0, parch = 0, pclass = 3]</li>

 <li>[sex = male, age = 4, sibsp = 4, parch = 0, pclass = 3]</li>

 <li>[sex = male, age = 4, sibsp = 0, parch = 5, pclass = 3]</li>

 <li>[sex = male, age = 4, sibsp = 0, parch = 0, pclass = 1]</li>

 <li>[sex = male, age = 40, sibsp = 0, parch = 0, pclass = 3]</li>

 <li>[sex = male, age = 40, sibsp = 4, parch = 0, pclass = 3]</li>

 <li>[sex = male, age = 40, sibsp = 0, parch = 5, pclass = 3]</li>

 <li>[sex = male, age = 40, sibsp = 0, parch = 0, pclass = 1]</li>

 <li>[sex = female, age = 4, sibsp = 0, parch = 0, pclass = 3]</li>

 <li>[sex = female, age = 4, sibsp = 4, parch = 0, pclass = 3]</li>

 <li>[sex = female, age = 4, sibsp = 0, parch = 5, pclass = 3]</li>

 <li>[sex = female, age = 4, sibsp = 0, parch = 0, pclass = 1]</li>

 <li>[sex = female, age = 40, sibsp = 0, parch = 0, pclass = 3]</li>

 <li>[sex = female, age = 40, sibsp = 4, parch = 0, pclass = 3]</li>

 <li>[sex = female, age = 40, sibsp = 0, parch = 5, pclass = 3]</li>

 <li>[sex = female, age = 40, sibsp = 0, parch = 0, pclass = 1]</li>

</ol>

<strong><u>Part (B):</u></strong>  Use <strong><u>Logistic Regression</u></strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>

<strong><u> </u></strong>

<strong><u>Part (C):</u></strong>  Use <strong><u>K Nearest Neighbor Classification</u></strong> with <strong>7 neighbors</strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>




<strong><u>Part (D):</u></strong>  Use <strong><u>Support Vector Machine (SVM) Classification</u></strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>




<strong><u>Part (E):</u></strong>  Use <strong><u>Kernel Support Vector Machine (K-SVM) Classification</u></strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>




<strong><u>Part (F):</u></strong>  Use <strong><u>Naïve Bayes Classification</u></strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>




<strong><u> </u></strong>

<strong><u> </u></strong>

<strong><u> </u></strong>

<strong><u>Part (G):</u></strong>  Use <strong><u>Decision Tree Classification</u></strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>




<strong><u>Part (H):</u></strong>  Use <strong><u>Random Forest Classification</u></strong> with <strong>10 Decision Trees</strong> to predict if a passenger in the Test set will survive the accident

<ol>

 <li>Print the prediction and the corresponding ground truth in the Test set</li>

 <li>Print the Confusion Matrix</li>

 <li>Compute Accuracy</li>

 <li>Print and Tabulate the result for the data set given above</li>

</ol>




<strong><u>Summarize your observations in terms of:</u></strong>

<ol>

 <li>Tabulate the result of prediction from each of the models for the 16 dataset points</li>

</ol>

<table width="727">

 <tbody>

  <tr>

   <td width="105"><strong>Logical Regression</strong></td>

   <td width="105"><strong>K-Nearest Neighbors</strong></td>

   <td width="105"><strong>Support Vector Machines</strong></td>

   <td width="105"><strong>Kernel Support Vector Machine</strong></td>

   <td width="94"><strong>Naïve Bayes</strong></td>

   <td width="102"><strong>Decision Tree</strong></td>

   <td width="112"><strong>Random Forest</strong></td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="94">[0]</td>

   <td width="102">[1]</td>

   <td width="112">[1]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="94">[0]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="94">[0]</td>

   <td width="102">[1]</td>

   <td width="112">[1]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="94">[1]</td>

   <td width="102">[1]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="94">[0]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="94">[0]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="94">[0]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="94">[0]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="94">[1]</td>

   <td width="102">[1]</td>

   <td width="112">[1]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="94">[0]</td>

   <td width="102">[1]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="94">[1]</td>

   <td width="102">[1]</td>

   <td width="112">[1]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="94">[1]</td>

   <td width="102">[1]</td>

   <td width="112">[1]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="94">[1]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[0]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="94">[0]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="94">[1]</td>

   <td width="102">[0]</td>

   <td width="112">[0]</td>

  </tr>

  <tr>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[1]</td>

   <td width="105">[0]</td>

   <td width="94">[1]</td>

   <td width="102">[1]</td>

   <td width="112">[1]</td>

  </tr>

  <tr>

   <td colspan="7" width="727"><strong>Accuracy Scores</strong></td>

  </tr>

  <tr>

   <td width="105"><strong>0.7847533632286996</strong><strong> </strong></td>

   <td width="105">0.7802690582959642</td>

   <td width="105">0.7802690582959642</td>

   <td width="105">0.6591928251121076</td>

   <td width="94">0.7757847533632287</td>

   <td width="102"><strong>0.9237668161434978</strong><strong> </strong></td>

   <td width="112"><strong>0.9282511210762332</strong><strong> </strong></td>

  </tr>

 </tbody>

</table>




<ol>

 <li>Which predictive models performed the best – Top 3</li>

</ol>

In boldface above

<ol>

 <li>What could possibly make the top 3 models outperform the rest?</li>

</ol>

Decision Trees and Random Forest are non-linear, whereas logistic regression works best with binary data.