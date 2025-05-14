---
title: CellsColor.Color
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and sets the RGB color
type: docs
url: /net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Gets and sets the RGB color.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: color.Color = Color.Red;
public void CellsColor_Property_Color()
{
    Workbook workbook = new Workbook();

    Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
    CellsColor color = workbook.CreateCellsColor();
    color.Color = Color.Red;
    range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);
    Cell cell = workbook.Worksheets[0].Cells["F5"];
    Style style = cell.GetStyle();
    Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.LeftBorder].LineStyle);
    Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.BottomBorder].LineStyle);
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.TopBorder].LineStyle);
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.RightBorder].LineStyle);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


