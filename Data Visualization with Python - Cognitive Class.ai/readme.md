---
## Module 1 - Important functions and key points

1. **sheet_name** parameter in **pd.read_excel** is for specifying the sheet name from the excel sheet which has to be imported as a Pandas Dataframe. If the name is not given, then the integers also work as reference for the sheet_number. 
2. Default format of **df.columns - pandas.core. indexes.base.Index       ||      df.index - pandas.core.indexes.range.RangeIndex**
3. **df.sum(axis = 1/0)** - Parameter of Axis better understanding (This is reverse to the general understanding of Axis parameter) 

Axis parameter in Pandas has a specific usage to define whether the operation has to be done w.r.t the rows or w.r.t the columns. 

> **(Axis = 0)** - Means that the operation has to be **performed over** the **Rows**. So when we perform df.sum with 0 as the axis. The sum operation is performed over the rows i.e all the values for the rows are added in **************************vertical manner.**************************
> 

> **(Axis  = 1)** - Means that the operation has to be **performed over** the **Columns**. So when we perform df.sum with 1 as the axis. The sum operation is performed over the columns i.e all the values for the columns are added in **************************horizontal manner.**************************
> 
1. **********************df.loc(value) -********************** Gets the data corresponding to the value mentioned. 
2. ******************df.iloc(index) -****************** Get the data corresponding to the index mentioned. 
3. **df.loc[’India’, [a,b,c,d…….]]** - The values are used as X & Y coordinates.
4. **plt.show( )** - Used to show the updates made to the visualization
5. **df.plot(kind=”line”)** - This plots the index column on the ******X-axis****** & the each **column as a different Line**
6. **df.sort_values(by=column_name, ascending = True/False)** - Sorts the dataset according to the given conditions

---

## Module 2 - Important functions and key points

1. Area plots are an extension of Line plots
2. **df.plot(kind = “area”, stacked=False, figsize=(x,y))** - This function can be used to plot Area plot using matplotlib and stacked = False is used to remove the opacity of the plot
3. **df.plot(kind = “area”, alpha = 0.35…)** - The alpha parameter in the plot function can be used to control the opacity of the area plot, more the value more the opacity.
4. **fig.set_xticks(bin_edges)** - Method to set x_ticks externally in seaborn (sns.histplot)
5. **count, bin_edges = np.histogram(df[’2013’])** - This is used to create bins from the data default 10 and get the edges for them which are known as ticks which can be set as the inidividual points or markers in a histogram on the X-axis
6. Multiple features histograms are important and must be having the following settings

```python
count, bin_edges = np.histogram(df_3, 15)

# Unstacked histogram
df_3.plot(kind="hist", 
          figsize=(10,6), 
          bins=15, 
          alpha=0.6, 
          xticks = bin_edges, 
          color=['coral', 'darkslateblue', 'mediumseagreen'], 
          stacked=True)

plt.title('Histogram of Immigration from Denmark, Norway, and Sweden from 1980 - 2013')
plt.ylabel('Number of Years')
plt.xlabel('Number of Immigrants')

plt.show()
```

7. **Annotations** can be used in plot function to mark important events on the plot using arrows or text.

---
