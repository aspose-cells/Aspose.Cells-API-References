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
// Called: Assert.IsFalse(chart.PlotArea.Border.IsVisible);
[Test]
        public void Property_IsVisible()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46558.ods");
            Chart chart = workbook.Worksheets["Einzel"].Charts[0];
            Assert.IsFalse(chart.ValueAxis.MajorGridLines.IsVisible);
            Assert.IsFalse(chart.PlotArea.Border.IsVisible);
            chart = workbook.Worksheets["Ausgewaehte"].Charts[0];
           AssertHelper.AreEqual(Color.FromArgb(255,255,153), chart.ValueAxis.MajorGridLines.Color);
            workbook.Save(Constants.destPath + "CELLSNET46558.xlsx");
        }
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


