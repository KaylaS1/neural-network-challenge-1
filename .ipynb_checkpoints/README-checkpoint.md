# Week 18 Kala Neural Network Challenge - Predict Student Loan Repayment

### Step 1: Preprocessing of data
* Read the input CSV file.
* Target column is "credit_ranking".
* Split input data into train and test.
* Used Standard Scalar to scale data.

### Step 2: Create the model
* Create a deep neural network using TensorFlow's Keras.
* Model has 2 hidden layers with 6 and 3 nodes.
* Model was trained using 50 epochs.
* Model was saved into a keras file.

### Step 3: Reload the model
* Model was reloaded using the saved keras file.
* Predictions were made on the test data.
* A classification report was generated on the test data and the predictions.

### Step 4 Conclusions:
1. Data needed to build a student loan recommendation system are as follows, explanation of each data element is provided inline.
* Loan amount - the larger the amount, the greater likelihood of default
* Course of study - a STEM degree or an MBA will result in a job with a greater likelihood of repayment
* Type of attendance - online, in person, hybrid - according to a survey of borrowers conducted by The Pew Charitable Trusts in 2021, students who attend exclusively online are more likely to default on their loan payment
* Part-time or Full-time attendance - according to the same survey mentioned above, part-time attendance also indicates a greater chance of default
* Completion of course - students who don't complete a course will likely not get a job and wil likely default
* Credit score - higher the score, greater the chance of repayment
* Student's income - higher the student's income, greater the chance of repayment
* Student's parents' income - higher the parents' or family income, greater the chance of repayment
* Student's family size - larger family sizes may result in more default
* Scholarships - increases chances of repayment
* Age - older students likely to be more responsible
* GPA - increased GPA will likely result in a job and therefore repayment

2. Based on the data, I would use a combination of **collaborative filtering and content-based filtering**, to make recommendations.
* For collaborative filtering, students with similar demographic data like family income, credit score and course of study are likely to have similar loan requirements and repayment histories.
* For content-based filtering, if a student has searched for loans before, or a specific type of loan, such students could be targeted for specific loan types.

3. Two real-world challenges:
* It would be difficult to track students down to find out what their income is, post-graduation.
* These days, most courses are partially online, so many courses could be considered as "hybrid".
 
### Sources of code and conclusions
* Most of my code is based on code provided in starter code file and in exercises by the AI Bootcamp.
* https://www.pewtrusts.org/en/research-and-analysis/articles/2024/01/30/borrowers-with-certain-educational-experiences-appear-more-likely-to-default