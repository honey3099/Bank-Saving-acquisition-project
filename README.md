The head of analytics is back. He has now prepared a much larger dataset that provides information on a local bank's marketing campaign. 
Our task is to predict whether someone will open a savings account. You will find more details about the dataset in the data section.


This project has 3 parts: 1) Building the best model you can and testing it in Kaggle (The final Pynb File),  2) Reporting your thinking through an executive summary (PPT File), and
3) the Outcome file (submission file)

Model Evaluation
We will evaluate models using Area under ROC (AUC).

AUC is commonly used to compare model accuracy. The maximum value that can be achieved is 1 (perfect model/classifier). 
An AUC value of 0.5 means that it performs equally to a random classifier. An AUC below a value of 0.5 means your model performs worse than a random one. 



Submission files is .csv files. They have to contain two columns: Id and outcome. 
Every customer in the given dataset has a unique customer ID under the Id column, as you can obtain it from the test.csv file.
where outcome is the predicted probability of being class 1 (opened saving account) and idis the customer ID. 



Executive Summary PPT: It includes the following topics:
1. Data understanding (visualization, etc.)
2. Data preparation (variable treatment, feature creation)
3. Modeling (what model did we use)
4. Evaluation methodology (how did we evaluate our model)
5. Managerial implications




Dataset Description:
We have two datasets. train.csv is for training your model, and test.csv contains the information to predict. The submission has to be strictly in the format indicated in the sample_submission.csv.

Dataset description:
Files
train.csv - the training set
test.csv - the test set
sample_submission.csv - a sample submission file in the correct format (Note that the outcome has to be the class probabilities)

Columns:

Client information
id - client id (numeric)
age - age of client (numeric)
job - type of job (categorical: "admin.","artisan","entrepreneur", "housemaid", "management", "retired", "self-employed", "services", "student", "technician", "unemployed", "unknown")
civil - marital status of client (categorical: "divorced", "married", "single","unknown"; note: "divorced" means divorced or widowed)
education - education of client (categorical: "4K", "6K", "K9", "K12", "illiterate", "apprenticeship", "university", "unknown")
credit - has credit in default? (categorical: "no","yes","unknown")
hloan - has housing loan? (categorical: "no","yes","unknown")
ploan - has personal loan? (categorical: "no","yes","unknown")

Campaign details
ctype - contact communication type (categorical: "cellular","telephone")
month - last contact month of year (categorical: "jan", "feb", "mar", …, "nov", "dec")
day - last contact day of the week (categorical: "mon","tue","wed","thu","fri")
ccontact - current number of contacts performed during this campaign and for this client (numeric, includes last contact)
lcdays - number of days that passed by since client was last contacted by a previous campaign (numeric; 999 means client was not previously contacted)
pcontact - number of contacts performed before this campaign and for this client (numeric)
presult - outcome previous marketing campaigns (categorical: "failure","nonexistent","success")

Socioeconomic indicators
employment - employment variation rate - quarterly indicator (numeric)
cprice - consumer price index - monthly indicator (numeric)
cconf - consumer confidence index - monthly indicator (numeric)
euri3 - euribor 3 month rate - daily indicator (numeric)
employees - number of employees - quarterly indicator (numeric)
Outcome variable (target)
outcome - has the client opened a saving account? (binary: 1 = "yes", 0 = "no")
