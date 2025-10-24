##GridCell.SetStyle
GridCell method. Sets style to cell. To improve performanceimplement SetStyle method not implement Style property
## GridCell.SetStyle method
Sets style to cell. To improve performance,implement "SetStyle" method, not implement "Style" property.
```csharp
public void SetStyle(Style value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | style to be set. |
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
