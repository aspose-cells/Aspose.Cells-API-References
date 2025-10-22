##GridCell.GetFontColor
GridCell method. Gets cell font color. When change the coloryou should invoke SetFontColor method to set font color to cell
## GridCell.GetFontColor method
Gets cell font color. When change the color,you should invoke "SetFontColor" method, to set font color to cell.
```csharp
public Color GetFontColor()
```
### Return Value
return cell font color.
### Examples
```csharp
[C#]
GridCell cell = gridDesktop1.GetActiveWorksheet().Cells[0, 0];
Font font = new Font("Courier New", 8, FontStyle.Italic);
cell.SetFont(font);
Color color = cell.GetFontColor();
color = Color.Black;
cell.SetFontColor(color);
[Visual Basic]
Dim cell As GridCell =  gridDesktop1.GetActiveWorksheet().Cells(0, 0)
Dim font As Font =  New Font("Courier New",8,FontStyle.Italic)
cell.SetFont(font)
Dim color As Color =  cell.GetFontColor()
color = Color.Black
cell.SetFontColor(color)
```
### See Also
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
