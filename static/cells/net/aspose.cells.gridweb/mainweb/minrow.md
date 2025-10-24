##MainWeb.MinRow
MainWeb property. Gets or sets the minimum display row indexzero based of the web sheet. The control uses the smaller value of MinRow and sheet datas min row
## MainWeb.MinRow property
Gets or sets the minimum display row index(zero based) of the web sheet. The control uses the smaller value of MinRow and sheet data's min row.
```csharp
public int MinRow { get; set; }
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
