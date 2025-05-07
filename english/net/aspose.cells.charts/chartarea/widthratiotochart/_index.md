---
title: ChartArea.WidthRatioToChart
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets or sets the horizontal offset from its lower right corner column in units of ratio of the chart area
type: docs
url: /net/aspose.cells.charts/chartarea/widthratiotochart/
---
## ChartArea.WidthRatioToChart property

Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, chart.ChartArea.WidthRatioToChart);
[Test]
        public void Property_WidthRatioToChart()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts/ChartAPI/Bug-809662-CalloutsMisplaced.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.Calculate();

            Assert.AreEqual(1, chart.ChartArea.WidthRatioToChart);
            Assert.AreEqual(4000, chart.ChartArea.Height);

            Assert.AreEqual(2680, chart.PlotArea.Width);
#if !SKIA
            Assert.AreEqual(3219, chart.PlotArea.Height); //skiasharp is 3181
#endif
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


