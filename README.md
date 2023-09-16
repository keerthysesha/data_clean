# Ex-01_DS_Data_Cleaning
# AIM
        To read the given data and perform data cleaning and save the cleaned data to a file.
# Explanation
    Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect,
 incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data,
 but rather finding a way to maximize datasets accuracy without necessarily deleting the information.
# ALGORITHM
  STEP 1: Read the given Data
  STEP 2: Get the information about the data
  STEP 3: Remove the null values from the data
  STEP 4: Save the Clean data to the file
# CODE and OUTPUT
## DATA SET:
```
import pandas as pd
df=pd.read_csv("Data_set.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna (df['aired_on'].mode()[0])
df['original_network']=df[ 'original_network'].fillna (df['aired_on'].mode()[0])
df.head()
df['rating']=df['rating'].fillna (df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()
df['watchers']=df['watchers'].fillna (df['watchers'].median())
df.head()
df.info()
df.isnull().sum()
```
## LOAN DATA:
```
import pandas as pd
df=pd.read_csv("Loan_data.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['Loan_ID']=df['Loan_ID'].fillna(df['LoanAmount'].mode()[0])
df.head()
df['Dependents']=df['Dependents'].fillna (df['Dependents'].mode()[0])
df.head()
df['Gender']=df['Gender'].fillna (df['Gender'].mode()[0])
df.head()
df['Education']=df['Education'].fillna (df['Dependents'].mode()[0])
df.head()
df['Self_Employed']=df['Self_Employed'].fillna (df['Self_Employed'].mode()[0])
df.head()
df['LoanAmount']=df['LoanAmount'].fillna (df['LoanAmount'].mean())
df.head()
df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())
df.head()
df['Credit_History']=df['Credit_History'].fillna (df['Credit_History'].median())
df.head()
df.info()
df.isnull().sum()
```
# OUTPUT:
# DATA SET:
# DATA:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/55cc51da-00bb-4968-81d7-d082f26e3ff0)


# NON NULL BEFORE:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/2e7cf4f6-9d81-4906-a2f2-09c37b016711)


# NON NULL AFTER:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/15e05ef7-3ecc-4348-b69e-3b90816c4d70)


# LOAN DATA:
## DATA:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/760b66ad-e67b-48c8-8f81-4c4a4f46008c)


# NON NULL BEFORE:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/e477df14-b568-4bfb-8df5-301ea9d2e9a5)


# MODE:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/752b48c9-eec7-40e6-826a-277547ae6ef4)


# MEAN:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/67d16e36-9fc8-4cff-a9df-018ae1a28b86)


![image](https://github.com/keerthysesha/data_clean/assets/125575936/a7590c87-b87c-4807-90ec-c92a1bdba3a2)


![image](https://github.com/keerthysesha/data_clean/assets/125575936/caa0eb49-daa5-41a6-9833-2b808607dfad)


![image](https://github.com/keerthysesha/data_clean/assets/125575936/bb4c5e18-57de-4ad3-b378-bffef53b0ba1)


# MEDIAN:
![image](https://github.com/keerthysesha/data_clean/assets/125575936/b4a080a6-a06b-434d-9118-c3291b78f13a)


![image](https://github.com/keerthysesha/data_clean/assets/125575936/6d9a7246-2f43-4daf-b57f-a6624daa1a3e)

# NON NULL AFTER:

![image](https://github.com/keerthysesha/data_clean/assets/125575936/c95a1220-148e-420d-be3c-a07903424b9c)

## RESULT:
           Thus the given data is read,cleansed and the cleaned data is saved into the file.

