##Delegate SheetEventHandler
Represents the interface that intend to handle sheet events
## SheetEventHandler delegate
Represents the interface that intend to handle sheet events.
void **handleCellEvent**(Object sender, RowColumnEventArgs e);
```csharp
public delegate void SheetEventHandler(object sender, GridWorksheet sheet);
```
| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source of the event. |
| sheet | GridWorksheet | The related worksheet. |
### See Also
* class [GridWorksheet](../gridworksheet/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
