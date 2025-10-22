##GridCell.GetFont
GridCell method. Gets cell font. When change the font you should invoke SetFont method to set font to cell
## GridCell.GetFont method
Gets cell font. When change the font, you should invoke "SetFont" method, to set font to cell.
```csharp
public Font GetFont()
```
### Return Value
return copy of cell font.
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
