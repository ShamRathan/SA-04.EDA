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
# OUTPUT:
# Initial Dataframe:
![op](./outpic/1.png)
# KDE for all numeric variables of the Dataframe:
![op](./outpic/2.png)
## Basic KDE plot for Pclass column:
![op](./outpic/3.png)
## Basic KDE plot for Age column:
![op](./outpic/4.png)
## Basic KDE plot for Fare column:
![op](./outpic/5.png)
## Basic KDE plot for Survived column:
![op](./outpic/6.png)
## Basic KDE plot for SibSp column:
![op](./outpic/7.png)
# KDE on a category using MULTIPLE argument:
## Survived Vs Sex:
![op](./outpic/8.png)
## Fare Vs Sex:
![op](./outpic/9.png)
## Survived Vs Pclass:
![op](./outpic/10.png)
# KDE on a category using MULTIPLE argument(Using additional Parameter- stack):
## Survived Vs Sex
![op](./outpic/11.png)
## Fare Vs Sex
![op](./outpic/12.png)
## Survived Vs Pclass:
![op](./outpic/13.png)
## Fare Vs Pclass:
![op](./outpic/14.png)
# KDE on a category using MULTIPLE argument(Using additional Parameter- stack,line width):
## Survived Vs Sex:
![op](./outpic/15.png)
## Survived Pclass:
![op](./outpic/16.png)

## Bivariate KDE:
## Survived Vs SibSp:
![op](./outpic/17.png)
## Survived Vs Fare:
![op](./outpic/18.png)
## Age Vs Fare:
![op](./outpic/19.png)
## Age Vs Pclass:
![op](./outpic/20.png)

# <p align ='center'> Thank You </p>






