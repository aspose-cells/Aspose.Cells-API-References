##GridCell.SetFontColor
GridCell method. Sets font color to cell. To improve performanceimplement SetFontColor method not implement FontColor property
## GridCell.SetFontColor method
Sets font color to cell. To improve performance,implement "SetFontColor" method, not implement "FontColor" property.
```csharp
public void SetFontColor(Color color)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | font color to be set. |
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
