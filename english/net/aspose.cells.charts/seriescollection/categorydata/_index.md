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
// Called: Assert.AreEqual("=Sheet1!$B$5:$B$7", chart.NSeries.CategoryData);
[Test]
        public void Property_CategoryData()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42789.ods");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(ChartType.Column, chart.NSeries[0].Type);
            Assert.AreEqual("=Sheet1!$B$5:$B$7", chart.NSeries.CategoryData);
            workbook.Save(Constants.destPath + "CELLSJAVA42789.xlsx");
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


