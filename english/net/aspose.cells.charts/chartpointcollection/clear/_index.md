---
title: ChartPointCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: ChartPointCollection method. Remove all setting of the chart points
type: docs
url: /net/aspose.cells.charts/chartpointcollection/clear/
---
## ChartPointCollection.Clear method

Remove all setting of the chart points.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: chart.NSeries[0].Points.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestBubble_134989.xls");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].Name = "=C1";
            chart.NSeries[0].XValues = "B24";
            chart.NSeries[0].Values = "B26";
            chart.NSeries[0].BubbleSizes = "C2";

            chart.CategoryAxis.MinValue = 0;
            chart.CategoryAxis.MaxValue = 2;
            chart.CategoryAxis.MajorUnit = 1;
            chart.CategoryAxis.MinorUnit = 1;
            chart.NSeries.IsColorVaried = false;
            chart.NSeries[0].Points.Clear();

            workbook.Save(Constants.destPath + "TestBubble_134989.xls");
            workbook = new Workbook(Constants.destPath + "TestBubble_134989.xls");
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.MaxValue, 2);
        }
```

### See Also

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


