---
title: Workbook.CreateCellsColor
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Creates a CellsColor object
type: docs
url: /net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Creates a [`CellsColor`](../../cellscolor/) object.

```csharp
public CellsColor CreateCellsColor()
```

### Return Value

Returns a [`CellsColor`](../../cellscolor/) object.

### Examples

```csharp
// Called: CellsColor color = workbook.CreateCellsColor();
[Test]
        public void Method_CreateCellsColor()
        {
            Workbook workbook = new Workbook();

            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.LeftBorder].LineStyle);
            Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.BottomBorder].LineStyle);
            Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.TopBorder].LineStyle);
            Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.RightBorder].LineStyle);
            workbook.Save(Constants.destPath + "CELLSNET50422.xlsx");
        }
```

### See Also

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


