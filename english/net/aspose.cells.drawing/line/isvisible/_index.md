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
// Called: chart.ValueAxis.MajorGridLines.IsVisible = true;
[Test]
        public void Property_IsVisible()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestGridline_001.xls&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsFalse(chart.ValueAxis.MajorGridLines.IsVisible);
            chart.ValueAxis.MajorGridLines.IsVisible = true;
            chart.ValueAxis.MinorGridLines.IsVisible = true;

            workbook.Save(Constants.destPath + &quot;TestGridline_001.xls&quot;);
        }
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


