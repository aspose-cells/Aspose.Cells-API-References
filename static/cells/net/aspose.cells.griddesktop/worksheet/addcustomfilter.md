##Worksheet.AddCustomFilter
Worksheet method. Add custom filter for the specified row range from start row to end row
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}
Add custom filter for the specified row range from start row to end row.
```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras,
GridFilterOperatorType[] filterOperatorTypes)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startrow | Int32 | The startrow of the filter range |
| startcolumn | Int32 | The startcolumn of the filter range |
| critiras | Object[] | The critira array for the columns,each one apply to each column |
| filterOperatorTypes | GridFilterOperatorType[] | The filter operate type array for the columns,each one apply to each column |
### See Also
* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## AddCustomFilter(int, string) {#addcustomfilter_1}
Add custom filter for the specified row.
```csharp
public void AddCustomFilter(int row, string critira)
```
### Remarks
The filter criteria string. notice we use , and ; as split char,so the cell value shall not contains with those split char below are the criteria string examples: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
