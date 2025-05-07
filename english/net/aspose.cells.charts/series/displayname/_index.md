---
title: Series.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the seriess name that displays on the chart graph
type: docs
url: /net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Gets the series's name that displays on the chart graph.

```csharp
public string DisplayName { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].DisplayName, "One");
[Test]
        public void Property_DisplayName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet42872.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.Calculate();
            Assert.AreEqual(chart.NSeries[0].DisplayName, "One");
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


