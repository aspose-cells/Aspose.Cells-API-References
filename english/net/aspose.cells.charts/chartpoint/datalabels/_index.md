---
title: ChartPoint.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Returns a DataLabels object that represents the data label associated with this chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Returns a `DataLabels` object that represents the data label associated with this chart point.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: DataLabels l = resultPoints[1].DataLabels;
[Test]
        public void Property_DataLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava45341.xlsx");
            Worksheet wordsheet = workbook.Worksheets[1];
            Chart chart = wordsheet.Charts[0];
            Series resultSeries = chart.NSeries[0];
            resultSeries.Values = ("=Sheet1!D3:D5");
            ChartPointCollection resultPoints = resultSeries.Points;
            DataLabels l = resultPoints[1].DataLabels;
            workbook.Save(Constants.destPath + "CellsJava45341.xlsx");

            Workbook workbook2 = new Workbook(Constants.destPath + "CellsJava45341.xlsx");
            workbook2.Save(Constants.destPath + "CellsJava45341.xlsx");
            workbook2 = new Workbook(Constants.destPath + "CellsJava45341.xlsx");
            chart = workbook2.Worksheets[1].Charts[0];
            Assert.IsTrue(chart.NSeries[0].Points[0].Area.InvertIfNegative);
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(0xed, 0x7d, 0x31), chart.NSeries[0].Points[0].Area.BackgroundColor));
        }
```

### See Also

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


