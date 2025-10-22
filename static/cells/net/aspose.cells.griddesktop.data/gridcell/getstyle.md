##GridCell.GetStyle
GridCell method. Gets cell style. When change the styleyou should invoke SetStyle method to set style to cell
## GridCell.GetStyle method
Gets cell style. When change the style,you should invoke "SetStyle" method, to set style to cell.
```csharp
public Style GetStyle()
```
### Return Value
return copy of cell style.
### Examples
```csharp
[C#]
Style style = sheet.GetCell(0, 0).GetStyle();
style.CellLocked = true;
style.VAlignment = VerticalAlignmentType.Top;
...
sheet.GetCell(0, 0).SetStyle(style);
[Visual Basic]
Dim style As Style =  sheet.GetCell(0,0).GetStyle()
style.CellLocked = True
style.VAlignment = VerticalAlignmentType.Top
...
sheet.GetCell(0, 0).SetStyle(style)
```
### See Also
* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
