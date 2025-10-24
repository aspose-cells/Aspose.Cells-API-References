##Delegate CellEventHandler
Represents the interface that intend to handle cell events
## CellEventHandler delegate
Represents the interface that intend to handle cell events.
void **handleCellEvent**(Object sender, CellEventArgs e);
```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```
| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source grid of the event. |
| e | CellEventArgs | The event argument. The e.Cell is the cell who fires the event. The e.Argument contains the argument of the event. |
### See Also
* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)
