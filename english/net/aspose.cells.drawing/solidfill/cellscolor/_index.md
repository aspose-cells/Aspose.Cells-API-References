---
title: SolidFill.CellsColor
second_title: Aspose.Cells for .NET API Reference
description: SolidFill property. Gets and sets the CellsColor object
type: docs
url: /net/aspose.cells.drawing/solidfill/cellscolor/
---
## SolidFill.CellsColor property

Gets and sets the `CellsColor` object.

```csharp
public CellsColor CellsColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].Area.FillFormat.SolidFill.CellsColor.ThemeColor.Tint, 0.6);
public void SolidFill_Property_CellsColor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    CellsColor cc = chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor;
    cc.ThemeColor = new ThemeColor(ThemeColorType.Accent6, 0.6);
    chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor = cc;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].Area.FillFormat.SolidFill.Color.ToArgb() & 0xFFFFFF, Color.FromArgb(252, 213, 181).ToArgb() & 0xFFFFFF);
    Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].Area.FillFormat.SolidFill.CellsColor.ThemeColor.Tint, 0.6);
}
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


