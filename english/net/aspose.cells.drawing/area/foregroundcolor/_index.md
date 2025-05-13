---
title: Area.ForegroundColor
second_title: Aspose.Cells for .NET API Reference
description: Area property. Gets or sets the foreground Color
type: docs
url: /net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Gets or sets the foreground Color.

```csharp
public Color ForegroundColor { get; set; }
```

### Examples

```csharp
// Called: Color c2 = chart.NSeries[1].Area.ForegroundColor;
public void Area_Property_ForegroundColor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Color c1 = chart.NSeries[0].Area.ForegroundColor;
    Color c2 = chart.NSeries[1].Area.ForegroundColor;
    Assert.IsTrue(Util.CompareColor(c1, Color.FromArgb(79, 129, 189)));
    Assert.IsTrue(Util.CompareColor(c2, Color.FromArgb(192, 80, 77)));
}
```

### See Also

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


