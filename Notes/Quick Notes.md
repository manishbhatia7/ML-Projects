# Quick Notes
### Check the Duplicates
```
print(f'Duplicates in Train Set: {train.duplicated().sum()}, ({np.round(100*train.duplicated().sum()/len(train),1)}%)')
```

