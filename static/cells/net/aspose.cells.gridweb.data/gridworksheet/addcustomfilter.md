##GridWorksheet.AddCustomFilter
GridWorksheet method. Add custom filter for the specified row
## GridWorksheet.AddCustomFilter method
Add custom filter for the specified row.
```csharp
public void AddCustomFilter(int row, string critira)
```
### Remarks
The filter criteria string. notice we use , and ; as split char,so the cell value shall not contains with those split char below are the criteria string examples //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC
### See Also
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
