---
title: ChartCalculateOptions.UpdateAllPoints
second_title: Aspose.Cells for .NET API Reference
description: ChartCalculateOptions property. Whether update all data points when performing the chart calculation. Default False. When you want to get the value for each data point in the chart specifically set it to true. If this parameter is set to True the new data points may be generated when chart is calculated. This could make the Excel file larger
type: docs
url: /net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Examples

```csharp
// Called: calculateOptions.UpdateAllPoints = true;
[Test]
        public void Property_UpdateAllPoints()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-49093.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartPointCollection points = chart.NSeries[0].Points;
            Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text");
            Assert.AreEqual(null, points[1].DataLabels.Text, "DataLabel Text");
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;
            chart.Calculate(calculateOptions);
            Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text"); // rich has no chars
            Assert.AreEqual("200", points[1].DataLabels.Text, "DataLabel Text");
            Assert.AreEqual("150", points[2].DataLabels.Text, "DataLabel Text"); // rich contains chars
            workbook.Save(Constants.destPath + "CELLSNET-49093_Resave.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET-49093_Resave.xlsx");
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text");
            Assert.AreEqual("200", points[1].DataLabels.Text, "DataLabel Text");
            Assert.AreEqual("150", points[2].DataLabels.Text, "DataLabel Text");
            chart.Calculate(calculateOptions);
            points = chart.NSeries[0].Points;
            Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text");
            Assert.AreEqual("200", points[1].DataLabels.Text, "DataLabel Text");
            Assert.AreEqual("150", points[2].DataLabels.Text, "DataLabel Text");
        }
```

### See Also

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


