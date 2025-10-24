##Delegate WorkbookEventHandler
Represents the interface that intend to handle workbook events
## WorkbookEventHandler delegate
Represents the interface that intend to handle workbook events.
void **handleCellEvent**(Object sender, CellEventArgs e);
```csharp
public delegate void WorkbookEventHandler(object sender, CellEventArgs e);
```
| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source of the event. |
| e | CellEventArgs | The event argument. |
### See Also
* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
