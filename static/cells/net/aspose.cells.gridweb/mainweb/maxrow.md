##MainWeb.MaxRow
MainWeb property. Gets or sets the maximum display row indexzero based of the web sheet. The control uses the greater value of MaxRow and sheet datas max row
## MainWeb.MaxRow property
Gets or sets the maximum display row index(zero based) of the web sheet. The control uses the greater value of MaxRow and sheet data's max row.
```csharp
public int MaxRow { get; set; }
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
