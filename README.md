<h1>Tackling an open problem</h1>

For this homework the idea is to hone our skills on exploring and plotting a dataset. You can either work with the Pokemon dataset that was given or download your own. If you opt to download your own I recommend you use one of the datasets available on kaggle,

https://www.kaggle.com/datasets

As they tend to be found in a clean format and are generally free to use.

Largely, the main objective is learning how to search the internet for new implementations you want to use on your code helping you develop your self-confidence.

There's no right or wrong, pick a dataset you enjoy and try to have some fun.
If you need, use the notebook from the previous session as a guideline.

import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
pwd
season1_df = pd.read_csv('OW2.csv', sep=',')
print(season1_df)
season1_df['Skill Tier'].describe()
season1_df.keys()
season1_df.columns
season1_df.hist()
season1_df.plot.scatter(x='KDA Ratio',y='Win Rate, %')
season1_df.plot.scatter(x='KDA Ratio',y='Skill Tier')

#yes but it would be easier if each group had a mean data point. its hard to compare the groups to each other without it
season1_df.hist("Eliminations / 10min")
season1_df['Hero'].value_counts().plot(kind='pie')
season1_df["Pick Rate, %"].value_counts().plot(kind='pie')
season1_df["Win Rate, %"].value_counts().plot(kind='pie')
season1_df = pd.DataFrame(np.random.rand(10, 5), columns=["A", "B", "C", "D", "E"])

season1_df.plot.box();# homework2
