##GridWorksheet.FilterString
GridWorksheet method. Sets the filter for the column.notice we shall call AddAutoFilter before calling of filterString The filter criteria string. notice we use comma as split charso the cell value you want to filter shall not contains with comma filterString10123456 means column 10 shall contain 123 or 456 filterString10123 means column10 shall contain 123 the column indexvalue split with commaeg. 123456789 or abc
## GridWorksheet.FilterString method
Sets the filter for the column.notice we shall call AddAutoFilter before calling of filterString The filter criteria string. notice we use comma-&gt;"," as split char,so the cell value you want to filter shall not contains with comma filterString(10,"123,456") means column 10 shall contain 123 or 456, filterString(10,"123") means column10 shall contain 123 the column indexvalue split with comma,eg. 123,456,789 or abc
```csharp
public void FilterString(int column, string criteria)
```
### See Also
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
