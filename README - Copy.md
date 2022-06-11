# <p align ='center'> A08-IMPLEMENT KDE PLOT </p>
## Name     : S.SHAM RATHAN
## Reg.no   : 212221230093
## Dept     : AIDS
## Sa Assignment : 08.
-----------------------------------------------------------------------
## Program:
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("titanic_dataset.csv")
df
#Create KDE for all the numeric variables in dataframe
sns.kdeplot(data=df)
sns.kdeplot(data=df, x='Pclass')
sns.kdeplot(data=df, x='Age')
sns.kdeplot(data=df, x='Fare')
sns.kdeplot(data=df,x='Survived',hue='Sex')
sns.kdeplot(data=df,x='Fare',hue='Sex')
sns.kdeplot(data=df,x='Survived',hue='Age')
sns.kdeplot(data=df,x='SibSp',hue='Age')
sns.kdeplot(data=df,x='Survived',hue='Pclass')
#Stack KDE on a category using MULTIPLE argument
sns.kdeplot(data=df,x='Survived',hue='Sex',multiple='stack')
sns.kdeplot(data=df,x='Survived',hue='Sex',multiple='stack',linewidth=5,palette='Dark2',alpha=0.5)
sns.kdeplot(data=df,x='Fare',hue='Sex',multiple='stack')
sns.kdeplot(data=df,x='Survived',hue='Pclass',multiple='stack')
sns.kdeplot(data=df,x='Survived',hue='Pclass',multiple='stack',linewidth=5,palette='Dark2',alpha=0.5)
sns.kdeplot(data=df,x='Fare',hue='Pclass',multiple='stack')
#Create a bivariate KDE
sns.kdeplot(data=df, x='Survived',y='SibSp')
sns.kdeplot(data=df, x='Survived',y='Fare')
sns.kdeplot(data=df, x='Age',y='Fare')
sns.kdeplot(data=df, x='Age',y='Pclass')
```
## Output:
![output](./outpic/1.png)
![output](./outpic/2.png)
![output](./outpic/3.png)
![output](./outpic/4.png)
![output](./outpic/5.png)
![output](./outpic/6.png)
![output](./outpic/7.png)
![output](./outpic/8.png)
![output](./outpic/9.png)
![output](./outpic/10.png)
![output](./outpic/11.png)
![output](./outpic/12.png)
![output](./outpic/13.png)
![output](./outpic/14.png)
![output](./outpic/15.png)
![output](./outpic/16.png)
![output](./outpic/17.png)
![output](./outpic/18.png)
![output](./outpic/19.png)
![output](./outpic/20.png)

# <p align ='center'> Thank You </p>






