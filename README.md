# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
import pandas as pd

data=pd.read_csv(r"C:\Users\MIRDULA\Downloads\Data_set (1).csv")

print(data)

<img width="815" height="826" alt="image" src="https://github.com/user-attachments/assets/644ec88e-42f8-434e-a1e7-b1d6d4e709ca" />




df=pd.DataFrame(data)

print(df.isnull())

<img width="685" height="569" alt="image" src="https://github.com/user-attachments/assets/27591f3f-f43b-4f4d-bbfc-33802b0671be" />




df=pd.DataFrame(data)

print(df.isnull().sum())

<img width="300" height="225" alt="image" src="https://github.com/user-attachments/assets/47bd73da-7cdc-430b-8f2f-e733a72af16f" />




df.info

<img width="993" height="855" alt="image" src="https://github.com/user-attachments/assets/5fa56d22-25a4-46cf-9967-a044788c1f2d" />




import pandas as pd

data=pd.read_csv(r"C:\Users\MIRDULA\Downloads\Data_set (1).csv")

df=pd.DataFrame(data) 

dfd=df.dropna()

print("AFTER DROPNA")

print(dfd)

<img width="670" height="875" alt="image" src="https://github.com/user-attachments/assets/f130262d-e16d-4a35-b58b-04fcc5592e64" />




dfd=df.dropna(axis=1)

print("AFTER DROPNA")

print(dfd)

<img width="526" height="316" alt="image" src="https://github.com/user-attachments/assets/add21e6e-edac-4fe6-8155-5860f77b9b8b" />




dfd=df.dropna(axis=1,inplace=True)

print("AFTER DROPNA")

print(dfd)

<img width="508" height="44" alt="image" src="https://github.com/user-attachments/assets/9bb5f94a-b926-48a9-9b81-f54c1990d5d9" />




df=pd.DataFrame(data) 

df1=df.iloc[[1,3,5],[1,3]]

print(df1)

<img width="423" height="92" alt="image" src="https://github.com/user-attachments/assets/fe6806ef-995e-4b8b-af5b-37a0a3617496" />




dfd=df.dropna(axis=0)

print("AFTER DROPNA")

print(dfd)

<img width="660" height="324" alt="image" src="https://github.com/user-attachments/assets/4b403861-169c-4cc8-af34-aced8981acac" />




df=pd.DataFrame(data)

print(df.isnull().any())

<img width="343" height="213" alt="image" src="https://github.com/user-attachments/assets/2c513d3e-ffb1-4a9c-b8b9-9d5328d26a3e" />




dfd=df.fillna(0)

print("AFTER FILLNA")

print(dfd)

<img width="751" height="862" alt="image" src="https://github.com/user-attachments/assets/8f791821-8b2a-4090-908a-088ac60f19c6" />




dfd=df.fillna(method="ffill")

print("AFTER FILLNA")

print(dfd)

<img width="736" height="866" alt="image" src="https://github.com/user-attachments/assets/157897ee-e74e-4ce3-a0b9-4d12406fd09c" />




dfd=df.fillna(method="bfill")

print("AFTER FILLNA")

print(dfd)

<img width="738" height="866" alt="image" src="https://github.com/user-attachments/assets/15c45c2c-de2d-46b7-87c6-8cd8db916536" />




dfd=df.fillna({'show_name':'nandy','aired_on':'wednesday','original_network':'Jio','rating':7.5})

print("AFTER FILLNA")

print(dfd)

<img width="794" height="876" alt="image" src="https://github.com/user-attachments/assets/07337b90-46f2-4a89-a4a1-745ee47d2251" />




df.describe()

<img width="824" height="368" alt="image" src="https://github.com/user-attachments/assets/1874b7c5-be89-4ee1-9a6a-0d22c9b2a7bb" />



































# Result
          <<include your Result here>>
