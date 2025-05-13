---
title: Line.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents whether the line is visible
type: docs
url: /net/aspose.cells.drawing/line/isvisible/
---
## Line.IsVisible property

Represents whether the line is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[1].Charts[0].CategoryAxis.MajorGridLines.IsVisible);
public void Line_Property_IsVisible()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    Assert.IsTrue(workbook.Worksheets[1].Charts[0].CategoryAxis.MajorGridLines.IsVisible);
    Assert.AreEqual(workbook.Worksheets[1].Charts[0].ValueAxis.MajorTickMark, TickMarkType.Cross);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(workbook.Worksheets[1].Charts[0].CategoryAxis.MajorGridLines.IsVisible);
    Assert.AreEqual(workbook.Worksheets[1].Charts[0].ValueAxis.MajorTickMark, TickMarkType.Cross);
    Assert.AreEqual("=Tabellen!$C$20:$C$20", workbook.Worksheets[1].Charts[0].NSeries[0].Name);
}
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


