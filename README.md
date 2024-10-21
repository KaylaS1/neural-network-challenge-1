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
1. Data needed to build a student loan recommendation system are as follows:
* Loan amount - the larger the amount, the greater likelihood of default
* Course of study - a STEM degree or an MBA will result in a job with a greater likelihood of repayment
* Type of attendance - online, in person, hybrid - it seems online attendance has more default
* Part-time or Full-time attendance - it seems part-time attendance leads to more default
* Completion of course - students who don't complete a course will likely not get a job and wil likely default
* Credit score - higher the score, greater the chance of repayment
* Student's income - higher the student's income, greater the chance of repayment
* Student's parents' income - higher the parents' or family income, greater the chance of repayment
* Student's family size - larger family sizes may result in more default
* Scholarships - increases chances of repayment
* Age - older students likely to be more responsible
* GPA - increased GPA will likely result in a job and therefore repayment

2. Based on the data, I would use **collaborative filtering**, using user data to make recommendations. Students with similar demographic data like family income and credit score are likely to have similar loan repayment histories.

3. Two real-world challenges:
* It would be difficult to track students down to find out if they completed their college courses or what their income is.
* These days, most courses are partially online, so all students could pick type of attendance as "hybrid".
 
### Sources of code
* Most of my code is based on code provided in starter code file and in exercises by the AI Bootcamp.