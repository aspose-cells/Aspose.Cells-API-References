---
title: Series.DoughnutHoleSize
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size between 10 and 90 percent
type: docs
url: /net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(25, chart.NSeries[0].DoughnutHoleSize);
[Test]
        public void Property_DoughnutHoleSize()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava42787.ods&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(ChartType.Doughnut, chart.NSeries[0].Type);
            Assert.AreEqual(5, chart.NSeries[0].Points.Count);
           AssertHelper.AreEqual(Color.FromArgb(0xff420e), chart.NSeries[0].Points[1].Area.ForegroundColor);
            Assert.AreEqual(25, chart.NSeries[0].DoughnutHoleSize);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42789.xlsx&quot;);

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


