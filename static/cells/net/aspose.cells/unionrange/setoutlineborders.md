##UnionRange.SetOutlineBorders
UnionRange method. Sets out line borders around a range of cells
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}
Sets out line borders around a range of cells.
```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Border styles. |
| borderColors | Color[] | Border colors. |
### Remarks
Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}
Sets the outline borders around a range of cells with same border style and color.
```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Border style. |
| borderColor | Color | Border color. |
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
