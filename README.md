# ODD2023-DataScience-Ex-03
## Aim:
To read the given data and perform the univariate analysis with different types of plots.
## Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
## Algorithm:
## Step1:
Read the given data.
## Step2:
Get the information about the data.
## Step3:
Remove the null values from the data.
## Step4:
Mention the datatypes from the data.
## Step5:
Count the values from the data.
## Program:
```
Developed By : VASUNDRA SRI R
Register number: 212222230168
```
## Superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
## Diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
## Output:
## Superstore.csv
![WhatsApp Image 2023-09-23 at 8 52 31 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/42d7fd97-49d0-44be-ac1a-36ee03d7db3e)
![WhatsApp Image 2023-09-23 at 8 56 49 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/a855330f-4160-45ed-bf80-c32c256377c4)
![WhatsApp Image 2023-09-23 at 8 58 12 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/d99938be-f417-4692-8d53-ba8a2e50facd)
![WhatsApp Image 2023-09-23 at 8 58 12 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/c8f114a2-02c8-4b3f-9f93-95ca5e9fc50b)
![WhatsApp Image 2023-09-23 at 8 58 12 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/b787f7b9-9b58-4602-91ae-47bc84922def)
![WhatsApp Image 2023-09-23 at 8 58 53 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/7535b093-55f6-4c00-acb8-e702bbccc0bd)
![WhatsApp Image 2023-09-23 at 8 58 58 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/7981bce6-1d26-4580-9ffe-16fcdf0f4dec)
![WhatsApp Image 2023-09-23 at 8 59 01 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/cff5a2e4-1679-41c7-bd86-350b4862a08f)
![WhatsApp Image 2023-09-23 at 8 59 06 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/c42ede2b-365e-4881-a5d0-5ec45d43b0a0)
![WhatsApp Image 2023-09-23 at 8 59 10 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/a529d0ce-36f2-4fb1-9f3b-5332f0e4dee4)

## Diabetes.csv
![WhatsApp Image 2023-09-23 at 9 00 49 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/4b774b1d-7cd8-42fe-819f-1c26696d5548)
![WhatsApp Image 2023-09-23 at 9 00 49 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/f4ae882f-d1d0-42d7-9c8f-dd49e8a5e8b0)
![WhatsApp Image 2023-09-23 at 9 00 48 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/0622ff42-953f-4454-a576-f0fe295d74d5)
![WhatsApp Image 2023-09-23 at 9 00 46 AM](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/7c9c25c8-4f04-4e0d-84c4-dafd84a52bc4)
![WhatsApp Image 2023-09-23 at 9 00 46 AM (1)](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/7e02bb0c-4813-4ea5-8bb6-3332bf799211)
![WhatsApp Image 2023-09-23 at 9 00 48 AM (1)](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/7568ebe5-631c-4643-b7b0-2f917796bd80)
![box](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/edc43ca3-d82c-4d2f-a5b3-b76cf54ff030)
![count](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/5b14bfe8-527f-4758-b553-817792526d89)
![dist](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/c8ebc3f7-0e19-4442-841d-990e793ca966)
![hist](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/1bf72c57-337f-4a0b-9b33-06ce2e38067f)
![skew](https://github.com/vasundrasriravi/ODD2023-DataScience-Ex-03/assets/119393983/152ccd61-f3c5-4f47-894d-0bf302b1d8bc)

## RESULT:
Hence the univariate analysis is verified.


