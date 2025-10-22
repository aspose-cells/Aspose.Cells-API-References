##MainWeb.MaxColumn
MainWeb property. Gets or sets the maximum display column indexzero based of the web sheet. The control uses the greater value of MaxColumn and sheet datas max column
## MainWeb.MaxColumn property
Gets or sets the maximum display column index(zero based) of the web sheet. The control uses the greater value of MaxColumn and sheet data's max column.
```csharp
public int MaxColumn { get; set; }
```
### Examples
```csharp
[C#]
// Creates a 4x4 "display window".
GridWeb1.MinRow = 2;
GridWeb1.MaxRow = 5;
GridWeb1.MinColumn = 3;
GridWeb1.MaxColumn = 6;
[Visual Basic]
' Creates a 4x4 "display window".
GridWeb1.MinRow = 2
GridWeb1.MaxRow = 5
GridWeb1.MinColumn = 3
GridWeb1.MaxColumn = 6
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
