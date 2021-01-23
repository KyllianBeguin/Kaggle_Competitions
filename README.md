__Kaggle competition n°1 : Titanic__

Summary
- Preview of the competition
- Variable used
- Dataset processing pipline
- Machine Learning
- Conclusion
.
.
.
__Preview of the competition__

Link to the competition : https://www.kaggle.com/c/titanic

Goal : It is your job to predict if a passenger survived the sinking of the Titanic or not. For each in the test set, you must predict a 0 or 1 value for the variable.

Evaluation : Your score is the percentage of passengers you correctly predict. This is known as accuracy.
.
.
.
__Variable used__

In order to solve this problem, I will use the gender, the age and the embarked variable.

Why ?
 - Gender : Ladies could have a better chance of survival. At this time (1912), men helped more easily women than other men.
 - Age : Young people could have a better chance of survival. Children at first, for obvious reason of "protect the kids", but also young people that have are in a good shape (good body and health).
 - Embarked : I saw in the data that for the 3 port of embarkation, the number of people that embarked are different for each port. People that embarked at the biggest port of embarkation could have a better chance of survival as they represent the biggest amount of people in the data.

(Check Titanic_Overview.ipynb file to see the numbers and graphics)
.
.
.
__Dataset processing pipeline__

To delete the fewest lines, the 'Cabin' column had been droped and then the .dropna() function was used on the resulting dataset.
'Cabin' column has the bigger amount of NAs among all the column in the raw dataset (see Titanic_Overview.ipynb)

I then created dummies variables for the 3 entry variable. It makes a 0 and 1 matrix.
About Age, the variable had been cuted in 5 slices with equal range. Then dummies was created.

From this dataset, the independant variable (the dummies) were added in another dataset
To extract the dependeant variable, I ask the dataset if a 'Survived' column exist. If so, it is extracted.
If not, the first column is extracted (should be the passenger ID)
.
.
.
__Machine Learning__

The KNN algorithm was used to solve the problem, out of the output from the pipeline dataset
KNN stands for 'k-nearest neighbors'. Here, it is used for classification.

According to my knowledge from my online course, it is a popular algorithm, This is the main reason why it was choosed.

3 nearest neighbors was choosed for this algorithm. As no data on survivability was provided from Kaggle, no quality test was operated.

for more information about KNN, please check the Wikipedia web pag at https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm
.
.
.
__Conclusion__

This was my first Kaggle competition, I really liked it !
As I was working at home for my formation, I did not payed any attention to this competition, even if I started it on December 10th (omg, so slow...)

But This formation really got me in the machine learning and I enjoy it ! I still struggle with the math and the algorithm (yeah I know it's important) but still, I am fascinated by this predictions from my computer !

Thank you for reading it, I look forward to complete other competitions and also more personnal projects !
