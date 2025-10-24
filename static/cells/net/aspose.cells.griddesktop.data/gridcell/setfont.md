##GridCell.SetFont
GridCell method. Sets font to cell. To improve performanceimplement SetFont method not implement Font property
## GridCell.SetFont method
Sets font to cell. To improve performance,implement "SetFont" method, not implement "Font" property.
```csharp
public void SetFont(Font font)
```
| Parameter | Type | Description |
| --- | --- | --- |
| font | Font | font to be set. |
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
