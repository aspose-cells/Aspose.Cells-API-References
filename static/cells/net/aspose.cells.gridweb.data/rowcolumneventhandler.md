##Delegate RowColumnEventHandler
Represents the interface that intend to handle row/column events
## RowColumnEventHandler delegate
Represents the interface that intend to handle row/column events.
void **handleCellEvent**(Object sender, RowColumnEventArgs e);
```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```
| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source of the event. |
| e | RowColumnEventArgs | The event argument. Call e.RejectOperation() if you want to cancel the deleting operation in RowDeleting or ColumnDeleting event handlers. |
### See Also
* class [RowColumnEventArgs](../../aspose.cells.gridweb/rowcolumneventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
