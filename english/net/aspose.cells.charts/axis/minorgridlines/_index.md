---
title: Axis.MinorGridLines
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents minor gridlines on a chart axis
type: docs
url: /net/aspose.cells.charts/axis/minorgridlines/
---
## Axis.MinorGridLines property

Represents minor gridlines on a chart axis.

```csharp
public Line MinorGridLines { get; }
```

### Examples

```csharp
// Called: chart.ValueAxis.MinorGridLines.IsVisible = true;
[Test]
        public void Property_MinorGridLines()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "TestGridline_001.xls");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsFalse(chart.ValueAxis.MajorGridLines.IsVisible);
            chart.ValueAxis.MajorGridLines.IsVisible = true;
            chart.ValueAxis.MinorGridLines.IsVisible = true;

            workbook.Save(Constants.destPath + "TestGridline_001.xls");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


