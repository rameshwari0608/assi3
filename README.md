# assi3
import plotly.express as px
import pandas as pd
df=pd.read_csv("Average_Daily_Traffic_Counts.csv",index_col=1)
print(df)
fig = px.bar(df, x = 'Vehicle Volume By Each Direction of 
Traffic', y = 'Boundaries - ZIP Codes')
l1 = px.line(df, x = 'Vehicle Volume By Each Direction of 
Traffic', y = 'Boundaries - ZIP Codes')
s1 = px.scatter(df, x = 'Vehicle Volume By Each Direction of 
Traffic', y = 'Boundaries - ZIP Codes')
fig.show()
l1.show()
s1.show()
/*
Traffic Volume Count Location Address ... 
5838 West 414.0 ... 52.0
320 East 176.0 ... 31.0
835 North 715.0 ... 22.0
125 East 316.0 ... 48.0
2924 East 1294.0 ... 47.0
... ... ... ...
[1279 rows x 14 columns]
