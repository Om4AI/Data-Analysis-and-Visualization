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
