##Enum SessionMode
Aspose.Cells.GridWeb.SessionMode enum. Represents the session mode of the grid
## SessionMode enumeration
Represents the session mode of the grid.
```csharp
public enum SessionMode
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Session | `0` | Uses the system session to store/recover the grid's sheet data automatically. |
| ViewState | `1` | Uses the page's viewstate to store/recover the grid's sheet data automatically. |
| Custom | `2` | Uses the LoadCustomData event to load the grid's sheet data manually. And uses the SheetDataUpdated event to save the grid's sheet data. |
| File | `3` | Uses the system file to store/recover the grid's sheet data automatically,user need to set SessionStorePath to specify the file directory. |
### See Also
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)
