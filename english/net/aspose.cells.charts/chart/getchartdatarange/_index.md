---
title: Chart.GetChartDataRange
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Gets the data source range of the chart
type: docs
url: /net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

Gets the data source range of the chart.

```csharp
public string GetChartDataRange()
```

### Return Value

The data source.

### Remarks

Only supports range.

### Examples

```csharp
// Called: String str = chart.GetChartDataRange();
[Test]
        public void Method_GetChartDataRange()
        {
            //=Sheet1!$A$1:$D$4
            //=Sheet1!$B$2:$D$2
            // = Sheet1!$A$1:$D$4
            //  = Sheet1!$B$2:$B$4
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET47806_40624.xlsx");

            Chart chart = workbook.Worksheets[0].Charts[0];

            String str = chart.GetChartDataRange();

            Assert.AreEqual("=Sheet1!$A$1:$D$4", str);
            Assert.AreEqual("=Sheet1!$B$2:$D$2", chart.NSeries[0].Values);


            chart.SwitchRowColumn();

            Assert.AreEqual("=Sheet1!$A$1:$D$4", str);
            Assert.AreEqual("=Sheet1!$B$2:$B$4", chart.NSeries[0].Values);
            workbook.Save(Constants.destPath + "CELLSNET47806_40624.xlsx");
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


