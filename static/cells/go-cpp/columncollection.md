##ColumnCollection Class
'ColumnCollection class. Encapsulates the object that represents columncollection in Go.'
## ColumnCollection class
Collection of the <see cref="Column"/> objects that represent the individual column(setting)s in a worksheet.The Column object only represents the settings such as column width, styles, .etc. for the whole column,has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column.And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection,has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.
```go
type ColumnCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetColumnByIndex](./getcolumnbyindex/) | Gets the Column object by the position in the list. |
|[Get](./get/) | Gets a Column object by column index.The Column object of given column index will be instantiated if it does not exist before. |
|[GetCount](./getcount/) |  |
