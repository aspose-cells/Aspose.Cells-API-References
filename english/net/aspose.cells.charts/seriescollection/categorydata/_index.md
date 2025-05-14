---
title: SeriesCollection.CategoryData
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Gets or sets the range of category Axis values. It can be a range of cells such as d1e10 or a sequence of values such as26810
type: docs
url: /net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Examples

```csharp
// Called: testAreEqual("=Sheet1!$A$1:$A$17", chart.NSeries.CategoryData, caseName);
private void SeriesCollection_Property_CategoryData(Workbook workbook)
        {
            Chart chart = workbook.Worksheets["Sheet1"].Charts[0];
            testAreEqual("=Sheet1!$E$3:$E$19", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$D$3:$D$19", chart.NSeries.CategoryData, caseName);

            chart = workbook.Worksheets["Chart1"].Charts[0];
            testAreEqual("=Sheet1!$B$1:$B$17", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$A$1:$A$17", chart.NSeries.CategoryData, caseName);

            chart = workbook.Worksheets["Sheet2"].Charts[0];
            testAreEqual("=Sheet1!$B$1:$B$17", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$A$1:$A$17", chart.NSeries.CategoryData, caseName);
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


