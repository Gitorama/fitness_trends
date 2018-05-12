  For this project, I was trying to predict a person's activeness levels(number of steps they took daily) from features such as hours 
of sleep, number of calories burned etc. I used a Kaggle dataset that showed the step count of an individual based on several factors. 
The dataset consisted of 96 rows and 7 columns. The columns consisted of the person's step count, the date recorded, mood, calories burned,
hours of sleep, bool_of_active(activeness rating), and weight in kilograms. 
  I first cleaned all of the data, which also included extracting the month out of the date column, making the month a separate column,
and then deleting the date column. My 6 features included the month, mood, calories burned, hours of sleep, bool_of_active, and weight
in kilograms and my target column became the step count. After cleaning, I used sklearn's resample function to bootstrap the data to a 
1000 rows so that I will have sufficient amounts of data for my training and test data. I then did an 80/20 split, and Regression was the machine
learning technique to use as I was dealing with a range of values for my target column(step count), however, when I tried to build a 
linear regression model from the data, it gave me a very low prediction accuracy of around 4%. And using any classification technique was
out of question as the baseline for the target column was at around 3%. I finally concluded that more data was needed in order to better
predict a person's step count, such as workout type, workout time, and meals for the day.
