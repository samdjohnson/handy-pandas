# handy-pandas
Tips and tricks to make manipulating data in Pandas easier

All tips assume pandas is imported as pd. For examples where the data frame is not defined, assume there is a data frame declared called df.

### Convert a column to a datetime

```python
df['datetime_column_name'] = pd.to_datetime(df['datetime)column_name'])
```

### Pickle a data frame to store on disk and read later

```python
df.to_pickle('file_path.pickle')
df = pd.read_pickle('file_path.pickle)
