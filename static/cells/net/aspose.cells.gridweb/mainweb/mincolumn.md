##MainWeb.MinColumn
MainWeb property. Gets or sets the minimum display column indexzero based of the web sheet. The control uses the smaller value of MinColumn and sheet datas min column
## MainWeb.MinColumn property
Gets or sets the minimum display column index(zero based) of the web sheet. The control uses the smaller value of MinColumn and sheet data's min column.
```csharp
public int MinColumn { get; set; }
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
