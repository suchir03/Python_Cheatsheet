### Pandas dataframe information code
```python

df = pd.read_csv(<filename>)

df.info(verbose:(bool|None)=None) # Provides columns info and data types
df.shape #provides rows x columns
df.size #provdies length for series and row multiplied by columns for dataframes
df.describe() # provides generic statistics

```
