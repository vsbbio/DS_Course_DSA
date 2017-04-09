## [Pandas]("http://pandas.pydata.org")

"To work with series and data frames"

## Series "It's unidimensional array with data and labels/index"
### Creating

1. SeriesObj = Series([1,2,3], index=[], columns=[])
2. SeriesObj.name = "SeriesName"
3. SeriesObj.index.name = "IndexSeriesName"


### Object type, format and others attributes
''
1. type(SeriesObj) => pandas.core.series.Series
2. SeriesObj.values => It returns only the data
3. SeriesObj.index => It returns the function which generate the index (e.g.) RangeIndex(start=0,stop=4,step=1)


## DataFrames

### Creating/Converting

1. df = pd.DataFrame(data)
2. df.to_csv(,sep = ",") | .to_excel
3. pd.read_excel(name, sheet_name="Name") | .read_csv
4. 




### Object type, format and others attributes

1. type(df) => pandas.core.frame.DataFrame
2. dfName.describe() => It returns a DataFrame's summary


### Other Functions

1. pd.isnull(dfName)

2. pd.notnull(dfName)

3. pd.set_index(values)

4. dfName.head()

5. pd.date_range("20160101", periods= 10, freq ="S" | "A" | "M")

6. df.mean()

7. df.apply(FunctionName)

8. df.merge(dfNames, on = KeyNameToMerge)

