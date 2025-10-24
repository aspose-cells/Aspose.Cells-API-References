##LoadFilter Class
'LoadFilter class. Encapsulates the object that represents loadfilter in Go.'
## LoadFilter class
Represents the filter that provides options for loading data when loading workbook from template.
```go
type LoadFilter struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLoadFilter](./newloadfilter/) | Constructs one LoadFilter with default filter options LoadDataFilterOptions::All. |
|[NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Constructs one LoadFilter with given filter options. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Gets the filter options to denote what data should be loaded. |
|[SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Sets the filter options to denote what data should be loaded. |
|[GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Specifies the sheets(indices) and order to be loaded.Default is null, that denotes to load all sheets in the default order in template file.If not null and some sheet's index is not in the returned array, then the sheet will not be loaded. |
|[StartSheet](./startsheet/) | Prepares filter options before loading given worksheet.User's implementation of LoadFilter can change the LoadDataFilterOptions hereto denote how to load data for this worksheet. |
