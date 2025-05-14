---
title: Range.SetInsideBorders
second_title: Aspose.Cells for .NET API Reference
description: Range method. Set inside borders of the range
type: docs
url: /net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Set inside borders of the range.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Inside borde type, only can be Vertical and Horizontal. |
| lineStyle | CellBorderType | The border style. |
| borderColor | CellsColor | The color of the border. |

### Examples

```csharp
// Called: range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);
public void Range_Method_SetInsideBorders()
{
    Workbook workbook = new Workbook();

    Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
    CellsColor color = workbook.CreateCellsColor();
    color.Color = Color.Red;
    range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);
    Cell cell = workbook.Worksheets[0].Cells["F5"];
    Style style = cell.GetStyle();
    Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.LeftBorder].LineStyle);
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.BottomBorder].LineStyle);
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.TopBorder].LineStyle);
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.RightBorder].LineStyle);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


