# Quick Notes
### Check the Duplicates
```
print(f'Duplicates in Train Set: {train.duplicated().sum()}, ({np.round(100*train.duplicated().sum()/len(train),1)}%)')
```

### Checking any columns for nullity
```
missing_columns=data.columns[data.isnull().any()]
print(f"Missing columns are {missing_columns.tolist()}")
```

### Check the no of unique values in dataframe
```
unique_values_df=pd.DataFrame({'Column name':cat_cols,'No of Unique Values':[data[col].nunique() for col in cat_cols]})
```