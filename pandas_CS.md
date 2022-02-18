#Python
## Pandas
### Dataframe information
df--> DatarFrame in variable df
ds--> DataSeries in variable ds
```python
df.info(verbose:(bool|None)=None) # Provides columns info and data types
df.shape #provides rows x columns
df.size #provdies length for series and row multiplied by columns for dataframes
df.describe() # provides generic statistics
df.dtypes #data types of each column

```
### Boolean Masking
df--> DatarFrame in variable df \n
ds--> DataSeries in variable ds

```python
df.<column_name> > 40.0 # df having column, the code will give all the values greater than 40 as True
df[df.<column_name> > 40.0] #Will give rows which are True (True which are greater than 40
```
or

```python
df[df.market_value.lt(40)] #Supports fill value
```
Pandas Method
<code>
.lt()
.le()
.gt()
.ge()
.eq()
 </code>

```python
df.market_value.between(20,40) # range boolean operation
df.market_value.isin(value)# value can be list or set
```

### Get unique values
df--> DatarFrame in variable df
ds--> DataSeries in variable ds
```python
df.<column_name>.unique() #Give unique values of that column
df.<column_name>.nunique() #Give the number of unique values; Excludes 'NaN'
ds.unique() #Series
ds.nunique() #Series; Excludes 'NaN'

```
