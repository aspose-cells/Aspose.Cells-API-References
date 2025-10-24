##WorksheetCollection.AddCopy
WorksheetCollection method. Adds a worksheet to the collection and copies data from an existed worksheet
## AddCopy(string) {#addcopy_1}
Adds a worksheet to the collection and copies data from an existed worksheet.
```csharp
public int AddCopy(string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |
### Return Value
[`Worksheet`](../../worksheet/) object index.
### Exceptions
| exception | condition |
| --- | --- |
| Exception | Specifies an invalid worksheet name. |
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## AddCopy(int) {#addcopy}
Adds a worksheet to the collection and copies data from an existed worksheet.
```csharp
public int AddCopy(int srcSheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| srcSheetIndex | Int32 | Index of source worksheet. |
### Return Value
[`Worksheet`](../../worksheet/) Index of of the new worksheet.
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
