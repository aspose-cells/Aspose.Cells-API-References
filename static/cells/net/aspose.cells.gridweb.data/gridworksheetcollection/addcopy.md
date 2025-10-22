##GridWorksheetCollection.AddCopy
GridWorksheetCollection method. Adds a worksheet to the collection and copies data from an existed worksheet
## AddCopy(string) {#addcopy_1}
Adds a worksheet to the collection and copies data from an existed worksheet.
```csharp
public int AddCopy(string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |
### Return Value
[`GridWorksheet`](../../gridworksheet/) object index.
### Exceptions
| exception | condition |
| --- | --- |
| CellsException | Specifies an invalid worksheet name. |
### See Also
* class [GridWorksheetCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## AddCopy(int) {#addcopy}
Adds a worksheet to the collection and copies data from an existed worksheet.
```csharp
public int AddCopy(int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index of source worksheet. |
### Return Value
[`GridWorksheet`](../../gridworksheet/) object index.
### See Also
* class [GridWorksheetCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
