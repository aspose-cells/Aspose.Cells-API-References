##Delegate CustomCommandEventHandler
Represents the interface that intend to handle Custom Command events
## CustomCommandEventHandler delegate
Represents the interface that intend to handle Custom Command events.
void **handleCellEvent**(Object sender, String command);
```csharp
public delegate void CustomCommandEventHandler(object sender, string command);
```
| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | The source grid of the event. |
| command | String | The command string user send. |
### See Also
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)
