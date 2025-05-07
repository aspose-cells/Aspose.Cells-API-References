---
title: Series.SplitValue
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart
type: docs
url: /net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```csharp
public double SplitValue { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, chart.NSeries[0].SplitValue);
[Test]
        public void Property_SplitValue()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "piepiechart_1.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsFalse(chart.NSeries[0].IsAutoSplit);
            Assert.AreEqual(3, chart.NSeries[0].SplitValue);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


